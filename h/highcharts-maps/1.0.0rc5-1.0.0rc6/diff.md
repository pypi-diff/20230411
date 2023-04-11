# Comparing `tmp/highcharts_maps-1.0.0rc5.tar.gz` & `tmp/highcharts_maps-1.0.0rc6.tar.gz`

## Comparing `highcharts_maps-1.0.0rc5.tar` & `highcharts_maps-1.0.0rc6.tar`

### file list

```diff
@@ -1,1481 +1,1485 @@
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.readthedocs.yaml
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.travis.yml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/CHANGES.rst
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/requirements.dev.txt
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/requirements.travis.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/requirements.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/setup.cfg
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tox.ini
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.github/workflows/pypi-test-publish.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/Makefile
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_contributors.rst
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_dependencies.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_installation.rst
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_support.rst
--rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_versus_alternatives.rst
--rw-r--r--   0        0        0    56205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api.rst
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/conf.py
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/contributing.rst
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/errors.rst
--rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/faq.rst
--rw-r--r--   0        0        0    34457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/glossary.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/history.rst
--rw-r--r--   0        0        0    16227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/index.rst
--rw-r--r--   0        0        0    24959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/license.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/links.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/make.bat
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/quickstart.rst
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/support.rst
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/testing.rst
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/toolkit.rst
--rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using.rst
--rw-r--r--   0        0        0    41670 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/visualizations.rst
--rw-r--r--   0        0        0    54859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/abands-example.png
--rw-r--r--   0        0        0    34552 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/ad-example.png
--rw-r--r--   0        0        0    43218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/apo-example.png
--rw-r--r--   0        0        0    87899 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/arcdiagram-example.png
--rw-r--r--   0        0        0    72487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/area-example.png
--rw-r--r--   0        0        0   124371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/arearange-example.png
--rw-r--r--   0        0        0    55288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/areaspline-example.png
--rw-r--r--   0        0        0    54998 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/aroon-example.png
--rw-r--r--   0        0        0    46438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/aroon-oscillator-example.png
--rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/atr-example.png
--rw-r--r--   0        0        0    20359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/awesome-oscillator-example.png
--rw-r--r--   0        0        0   485952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/axis-property-mapping.xlsx
--rw-r--r--   0        0        0    59173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/bar-example.png
--rw-r--r--   0        0        0    48934 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/bellcurve-example.png
--rw-r--r--   0        0        0    43491 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/bollinger-bands-example.png
--rw-r--r--   0        0        0    37690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/boxplot-example.png
--rw-r--r--   0        0        0    92954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/bubble-example.png
--rw-r--r--   0        0        0    26870 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/bullet-example.png
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/candlestick-example.png
--rw-r--r--   0        0        0    52121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/cci-example.png
--rw-r--r--   0        0        0    49536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/chaikin-example.png
--rw-r--r--   0        0        0    46772 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/cmf-example.png
--rw-r--r--   0        0        0    47632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/cmo-example.png
--rw-r--r--   0        0        0    41242 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/column-example.png
--rw-r--r--   0        0        0    41567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example-stacked-horizontal.png
--rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example-stacked.png
--rw-r--r--   0        0        0    51790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example.png
--rw-r--r--   0        0        0    63741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/columnrange-example-horizontal.png
--rw-r--r--   0        0        0    68246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/columnrange-example.png
--rw-r--r--   0        0        0    67368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/cylinder-example.png
--rw-r--r--   0        0        0    54030 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/dema-example.png
--rw-r--r--   0        0        0   252801 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/dependencywheel-example.png
--rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/disparity-index-example.png
--rw-r--r--   0        0        0    45925 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/dmi-example.png
--rw-r--r--   0        0        0    37726 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/dpo-example.png
--rw-r--r--   0        0        0    66693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/dumbbell-example.png
--rw-r--r--   0        0        0    38446 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/ema-example.png
--rw-r--r--   0        0        0    59876 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/errorbar-example.png
--rw-r--r--   0        0        0    27702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/flags-example.png
--rw-r--r--   0        0        0    43626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/funnel-example.png
--rw-r--r--   0        0        0    60815 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/funnel_3d-example.png
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/gantt-example.png
--rw-r--r--   0        0        0   129516 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/gauge-example.png
--rw-r--r--   0        0        0    87393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/heatmap-example.png
--rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/heikin-ashi-example.png
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/highcharts-for-python-dark-32x32.png
--rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/highcharts-for-python-light-150x149.png
--rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/highcharts-logo.svg
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/highcharts-python-logo.png
--rw-r--r--   0        0        0    38747 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/histogram-example.png
--rw-r--r--   0        0        0    25456 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/hlc-example.png
--rw-r--r--   0        0        0    34397 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/hollow-candlestick-example.png
--rw-r--r--   0        0        0    73793 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/ikh-example.png
--rw-r--r--   0        0        0   208287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/item-example-circular.png
--rw-r--r--   0        0        0   151954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/item-example-rectangular.png
--rw-r--r--   0        0        0    15447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/item-example-symbols.png
--rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/keltner-channels-example.png
--rw-r--r--   0        0        0    40750 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/klinger-example.png
--rw-r--r--   0        0        0    81283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/line-example.png
--rw-r--r--   0        0        0    59025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/linear-regression-angle-example.png
--rw-r--r--   0        0        0    58305 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/linear-regression-example.png
--rw-r--r--   0        0        0    54179 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/linear-regression-intercept-example.png
--rw-r--r--   0        0        0    53628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/linear-regression-slope-example.png
--rw-r--r--   0        0        0    47835 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/lollipop-example.png
--rw-r--r--   0        0        0    41461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/macd-example.png
--rw-r--r--   0        0        0   104539 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/map-example.png
--rw-r--r--   0        0        0   201616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/mapbubble-example.png
--rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/mapline-example.png
--rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/mappoint-example.png
--rw-r--r--   0        0        0    44732 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/mfi-example.png
--rw-r--r--   0        0        0    51251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/momentum-example.png
--rw-r--r--   0        0        0    49554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/natr-example.png
--rw-r--r--   0        0        0    53945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/navigator-example.png
--rw-r--r--   0        0        0   269275 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/networkgraph-example.png
--rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/obv-example.png
--rw-r--r--   0        0        0    34656 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/ohlc-example.png
--rw-r--r--   0        0        0    48433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/organization-example-horizontal.png
--rw-r--r--   0        0        0   106952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/organization-example.png
--rw-r--r--   0        0        0   265002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/packedbubble-example-split.png
--rw-r--r--   0        0        0   298951 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/packedbubble-example.png
--rw-r--r--   0        0        0    58765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pareto-example.png
--rw-r--r--   0        0        0    90797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pie-example-donut.png
--rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pie-example.png
--rw-r--r--   0        0        0    47842 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pivot-points-example.png
--rw-r--r--   0        0        0    56333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/polygon-example.png
--rw-r--r--   0        0        0    44413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/ppo-example.png
--rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/price-channel-example.png
--rw-r--r--   0        0        0    43588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/price-envelopes-example.png
--rw-r--r--   0        0        0    47048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/psar-example.png
--rw-r--r--   0        0        0    49049 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pyramid-example.png
--rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/pyramid_3d-example.png
--rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/range-selector-example.png
--rw-r--r--   0        0        0    49944 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/roc-example.png
--rw-r--r--   0        0        0    45958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/rsi-example.png
--rw-r--r--   0        0        0   197682 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sankey-example-inverted.png
--rw-r--r--   0        0        0    79510 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sankey-example-outgoing.png
--rw-r--r--   0        0        0   227684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sankey-example.png
--rw-r--r--   0        0        0   109494 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/scatter-example.png
--rw-r--r--   0        0        0    29303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/scatter_3d-example.png
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/shared_options.js
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/shared_options_output.js
--rw-r--r--   0        0        0    53177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/slow-stochastic-example.png
--rw-r--r--   0        0        0    50549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sma-example.png
--rw-r--r--   0        0        0    28628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/solidgauge-example.png
--rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sphinx_rtd_theme_ext_color_contrast.css
--rw-r--r--   0        0        0    81626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/spline-example.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/square-check-solid.svg
--rw-r--r--   0        0        0    41933 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/stochastic-example.png
--rw-r--r--   0        0        0    71303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/stock-tools-example.png
--rw-r--r--   0        0        0   278653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/streamgraph-example.png
--rw-r--r--   0        0        0   397432 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/sunburst-example.png
--rw-r--r--   0        0        0    34040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/supertrend-example.png
--rw-r--r--   0        0        0    55620 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/tema-example.png
--rw-r--r--   0        0        0   199024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/tilemap-example-circle.png
--rw-r--r--   0        0        0    95113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/tilemap-example-diamond.png
--rw-r--r--   0        0        0    81668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/tilemap-example.png
--rw-r--r--   0        0        0    33235 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/timeline-example-datetime.png
--rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/timeline-example-inverted.png
--rw-r--r--   0        0        0    13386 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/timeline-example.png
--rw-r--r--   0        0        0    59391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/treemap-example.png
--rw-r--r--   0        0        0    44325 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/trendline-example.png
--rw-r--r--   0        0        0    36104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/trix-example.png
--rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/variablepie-example.png
--rw-r--r--   0        0        0    10175 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/variwide-example-datetime.png
--rw-r--r--   0        0        0    28517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/variwide-example-inverted.png
--rw-r--r--   0        0        0    74616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/variwide-example.png
--rw-r--r--   0        0        0    93945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/vbp-example.png
--rw-r--r--   0        0        0   173850 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/vector-example.png
--rw-r--r--   0        0        0    58194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/venn-example-euler.png
--rw-r--r--   0        0        0    94796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/venn-example.png
--rw-r--r--   0        0        0    41570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/vwap-example.png
--rw-r--r--   0        0        0    59407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/waterfall-example-inverted.png
--rw-r--r--   0        0        0    12628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/waterfall-example-stacked.png
--rw-r--r--   0        0        0    59664 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/waterfall-example.png
--rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/williamsr-example.png
--rw-r--r--   0        0        0    67964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/windbarb-example.png
--rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/wma-example.png
--rw-r--r--   0        0        0   177320 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/wordcloud-example.png
--rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/xrange-example-inverted.png
--rw-r--r--   0        0        0    30421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/xrange-example.png
--rw-r--r--   0        0        0    64223 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/_static/zigzag-example.png
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_class_structures.rst
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_deserialization_methods.rst
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_handling_defaults.rst
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_module_structure.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_other_convenience_methods.rst
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/_serialization_methods.rst
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/chart.rst
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/headless_export.rst
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/highcharts.rst
--rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/internals.rst
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/index.rst
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/shared_options.rst
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/export_data.rst
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/index.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/navigation.rst
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/announce_new_data.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/axis.rst
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/chart_types.rst
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/exporting.rst
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/index.rst
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/legend.rst
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/range_selector.rst
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/screen_reader_section.rst
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/series.rst
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/sonification.rst
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/table.rst
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/zoom.rst
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/boost.rst
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/caption.rst
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/credits.rst
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/data.rst
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/defs.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/drilldown.rst
--rw-r--r--   0        0        0    39926 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/index.rst
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/loading.rst
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/map_navigation.rst
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/responsive.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/subtitle.rst
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/time.rst
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/title.rst
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/tooltips.rst
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/announce_new_data.rst
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/index.rst
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/point.rst
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/screen_reader_section.rst
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/series.rst
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/focus_border.rst
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/index.rst
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/animation.rst
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/control_point_options.rst
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/events.rst
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/index.rst
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/label_options.rst
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/points.rst
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/annotations/shape_options.rst
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/accessibility.rst
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/breaks.rst
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/color_axis.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/crosshair.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/data_classes.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/generic.rst
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/index.rst
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/labels.rst
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/markers.rst
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/numeric.rst
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/parallel_axes.rst
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/plot_bands.rst
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/title.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/x_axis.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/y_axis.rst
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/axes/z_axis.rst
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/chart/index.rst
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/chart/options_3d.rst
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/chart/reset_zoom_button.rst
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/chart/scrollable_plot_area.rst
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/chart/zooming.rst
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/exporting/csv.rst
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/exporting/index.rst
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/exporting/pdf_font.rst
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/legend/accessibility.rst
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/legend/bubble_legend.rst
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/legend/index.rst
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/legend/navigation.rst
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/legend/title.rst
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/map_views/index.rst
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/map_views/insets.rst
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/navigation/bindings.rst
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/navigation/index.rst
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/accessibility.rst
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/arcdiagram.rst
--rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/area.rst
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bar.rst
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/base.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bellcurve.rst
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/boxplot.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bubble.rst
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bullet.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/data_sorting.rst
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/dependencywheel.rst
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/drag_drop.rst
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/dumbbell.rst
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/funnel.rst
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/gauge.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/generic.rst
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/heatmap.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/histogram.rst
--rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/index.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/item.rst
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/levels.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/link.rst
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/map.rst
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mapbubble.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mapline.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mappoint.rst
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/networkgraph.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/organization.rst
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/packedbubble.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pareto.rst
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pie.rst
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/points.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/polygon.rst
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pyramid.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/sankey.rst
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/scatter.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/series.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/spline.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/sunburst.rst
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/timeline.rst
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/treemap.rst
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/vector.rst
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/venn.rst
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/plot_options/wordcloud.rst
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/arcdiagram.rst
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/area.rst
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/bar.rst
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/base.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/bellcurve.rst
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/boxplot.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/bubble.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/bullet.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/dependencywheel.rst
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/dumbbell.rst
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/funnel.rst
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/gauge.rst
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/heatmap.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/histogram.rst
--rw-r--r--   0        0        0    13470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/index.rst
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/item.rst
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/labels.rst
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/map.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/mapbubble.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/mapline.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/mappoint.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/networkgraph.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/organization.rst
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/packedbubble.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/pareto.rst
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/pie.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/polygon.rst
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/pyramid.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/sankey.rst
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/scatter.rst
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/series_generator.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/spline.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/sunburst.rst
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/timeline.rst
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/treemap.rst
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/vector.rst
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/venn.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/wordcloud.rst
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/accessibility.rst
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/arcdiagram.rst
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/bar.rst
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/base.rst
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/boxplot.rst
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/bullet.rst
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/cartesian.rst
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/connections.rst
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/geometric.rst
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/index.rst
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/map_data.rst
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/pie.rst
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/range.rst
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/single_point.rst
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/sunburst.rst
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/treemap.rst
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/vector.rst
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/venn.rst
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/options/series/data/wordcloud.rst
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/animation.rst
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/ast.rst
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/breadcrumbs.rst
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/buttons.rst
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/clusters.rst
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/data_grouping.rst
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/data_labels.rst
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/date_time_label_formats.rst
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/events.rst
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/fetch_configuration.rst
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/geojson.rst
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/gradients.rst
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/index.rst
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/javascript_functions.rst
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/jitter.rst
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/markers.rst
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/menus.rst
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/nodes.rst
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/partial_fill.rst
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/patterns.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/position.rst
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/projections.rst
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/shadows.rst
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/states.rst
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/topojson.rst
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/api/utility_classes/zones.rst
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/_code_style_naming_conventions.rst
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/_importing.rst
--rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/_working_with_maps_features.rst
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_add_series.rst
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_from_geopandas.rst
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_from_series.rst
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_series_property.rst
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_using_async_map_data.rst
--rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_using_synchronous_map_data.rst
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_with_chart_map.rst
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_with_series_map_data.rst
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/download_visualizations/_using_custom.rst
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/download_visualizations/_using_highsoft.rst
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_csv.rst
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_geopandas.rst
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_pandas.rst
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_pyspark.rst
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_csv.rst
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_geopandas.rst
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_pandas.rst
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_pyspark.rst
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_with_data_property.rst
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_with_from_array.rst
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/rendering_your_visualizations/_as_jupyter.rst
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/rendering_your_visualizations/_as_web_content.rst
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_dict.rst
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_js_literal.rst
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_json.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/templates/_with_copy.rst
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/templates/_with_dict.rst
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/templates/_with_js_literal.rst
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/docs/using/templates/_with_json.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/__version__.py
--rw-r--r--   0        0        0    51827 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/chart.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/constants.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/decorators.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/errors.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/headless_export.py
--rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/highcharts.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/js_literal_functions.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/metaclasses.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/__init__.py
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/shared_options.py
--rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/__init__.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/export_data.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/navigation.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/announce_new_data.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/axis.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/chart_types.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/exporting.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/legend.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/range_selector.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/screen_reader_section.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/series.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/sonification.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/table.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/accessibility/zoom.py
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/boost.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/caption.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/credits.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/data.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/defs.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/drilldown.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/loading.py
--rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/map_navigation.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/responsive.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/subtitle.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/time.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/title.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/tooltips.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/announce_new_data.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/high_contrast_theme.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/point.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/screen_reader_section.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/series.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/keyboard_navigation/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/keyboard_navigation/focus_border.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/accessibility/keyboard_navigation/series_navigation.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/__init__.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/animation.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/control_point_options.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/events.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/label_options.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/points.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/annotations/shape_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/accessibility.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/breaks.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/color_axis.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/crosshair.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/data_classes.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/generic.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/labels.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/markers.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/numeric.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/parallel_axes.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/plot_bands.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/title.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/x_axis.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/y_axis.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/axes/z_axis.py
--rw-r--r--   0        0        0    11460 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/__init__.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/options_3d.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/reset_zoom_button.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/scrollable_plot_area.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/zooming.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/exporting/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/exporting/csv.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/exporting/pdf_font.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/legend/__init__.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/legend/accessibility.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/legend/bubble_legend.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/legend/navigation.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/legend/title.py
--rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/map_views/__init__.py
--rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/map_views/insets.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/navigation/__init__.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/navigation/bindings.py
--rw-r--r--   0        0        0    53247 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/accessibility.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/arcdiagram.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/area.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/bar.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/bellcurve.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/boxplot.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/bubble.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/bullet.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/data_sorting.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/dependencywheel.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/drag_drop.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/dumbbell.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/funnel.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/gauge.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/generic.py
--rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/heatmap.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/histogram.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/item.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/levels.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/link.py
--rw-r--r--   0        0        0    17236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/map.py
--rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mapbubble.py
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mapline.py
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mappoint.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/networkgraph.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/organization.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/packedbubble.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/pareto.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/pie.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/points.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/polygon.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/pyramid.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/sankey.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/scatter.py
--rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/series.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/spline.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/sunburst.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/timeline.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/treemap.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/vector.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/venn.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/arcdiagram.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/area.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/bar.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/base.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/bellcurve.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/boxplot.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/bubble.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/bullet.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/dependencywheel.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/dumbbell.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/funnel.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/gauge.py
--rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/heatmap.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/histogram.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/item.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/labels.py
--rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/map.py
--rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mapbubble.py
--rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mapline.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mappoint.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/networkgraph.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/organization.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/packedbubble.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/pareto.py
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/pie.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/polygon.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/pyramid.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/sankey.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/scatter.py
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/series_generator.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/spline.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/sunburst.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/timeline.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/treemap.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/vector.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/venn.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/accessibility.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/arcdiagram.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/bar.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/base.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/boxplot.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/bullet.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/cartesian.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/connections.py
--rw-r--r--   0        0        0    22887 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/geometric.py
--rw-r--r--   0        0        0    26704 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/map_data.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/pie.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/range.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/single_point.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/sunburst.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/treemap.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/vector.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/venn.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/animation.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/ast.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/breadcrumbs.py
--rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/buttons.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/clusters.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/data_grouping.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/data_labels.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/date_time_label_formats.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/events.py
--rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/fetch_configuration.py
--rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/geojson.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/gradients.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/javascript_functions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/jitter.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/markers.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/menus.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/nodes.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/partial_fill.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/patterns.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/position.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/projections.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/shadows.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/states.py
--rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/topojson.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/zones.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/__init__.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/conftest.py
--rw-r--r--   0        0        0    37705 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/fixtures.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_chart.py
--rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_decorators.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_headless_export.py
--rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_js_literal_functions.py
--rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_metaclasses.py
--rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_mro.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/test_utility_functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/__init__.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/test_shared_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/__init__.py
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/test_export_data.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/test_language.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/test_navigation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/accessibility/__init__.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/accessibility/test_accessibility.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/global_options/language/accessibility/test_series.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/accessibility/accessibility/01.js
--rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/accessibility/accessibility/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/accessibility/accessibility/error-02.js
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/annotation/01.js
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/annotation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/annotation/error-02.js
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/01.js
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/02.js
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/03.js
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/04.js
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/05.js
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/06.js
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/07.js
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/08.js
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/09.js
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/10.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-01.js
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-02.js
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-03.js
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-04.js
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-05.js
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-06.js
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-07.js
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-08.js
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-09.js
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-10.js
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/01.js
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/02.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/error-01.js
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/error-02.js
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/01.js
--rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/02.js
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/error-01.js
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/error-02.js
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/01.js
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/02.js
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/error-01.js
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/error-02.js
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/01.js
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/02.js
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/error-01.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/error-02.js
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/resize/01.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/resize/error-01.js
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/01.js
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/02.js
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/error-01.js
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/error-02.js
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/01.js
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/02.js
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/error-01.js
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/error-02.js
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/01.js
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/02.js
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/error-01.js
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/error-02.js
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/boost/01.js
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/boost/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/boost/error-02.js
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/caption/01.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/caption/02.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/caption/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/caption/error-02.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/chart/01.js
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/chart/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/chart/error-02.js
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/options_3d/01.js
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/options_3d/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/options_3d/error-02.js
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/zooming/01.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart/zooming/error-01.js
--rw-r--r--   0        0        0   461024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart_obj/01-expected.js
--rw-r--r--   0        0        0   496450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/chart_obj/01-input.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/credits/01.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/credits/02.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/credits/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/credits/error-02.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/data/01.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/data/02.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/data/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/data/error-02.js
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/drilldown/01.js
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/drilldown/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/drilldown/error-02.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/csv/01.js
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/csv/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/csv/error-02.js
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/exporting/01.js
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/exporting/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/exporting/exporting/error-02.js
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/accessibility/01.js
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/accessibility/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/accessibility/error-02.js
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/01.js
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/02.js
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/error-02.js
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/error-03.js
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/export_data/01.js
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/export_data/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/export_data/error-02.js
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/language/01.js
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/language/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/language/error-02.js
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/01.js
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/02.js
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/error-02.js
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/error-03.js
--rw-r--r--   0        0        0   461353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/shared_options/01-expected.js
--rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/global_options/shared_options/01-input.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/headless_export/basic.json
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/headless_export/with-chart-type.js
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/headless_export/with-series-types.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/headless_export/output/placeholder.txt
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/bubble_legend/01.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/bubble_legend/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/bubble_legend/error-02.js
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/legend/01.js
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/legend/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/legend/error-02.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/navigation/01.js
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/legend/navigation/error-02.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/loading/01.js
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/loading/02.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/loading/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/loading/error-02.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/01.js
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/02.js
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/error-02.js
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/error-03.js
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/navigation/01.js
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/navigation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/navigation/navigation/error-02.js
--rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/options/01.js
--rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/01.js
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/error-02.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/01.js
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/error-00.js
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/error-01.js
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/error-02.js
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/01.js
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/02.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/03.js
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/04.js
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/05.js
--rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/06.js
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/07.js
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/08.js
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/09.js
--rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/10.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/error-02.js
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/01.js
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/error-00.js
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/error-01.js
--rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/error-02.js
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/01.js
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/error-02.js
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/01.js
--rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/error-02.js
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/01.js
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/error-00.js
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/error-01.js
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/error-02.js
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/01.js
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/error-02.js
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/01.js
--rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/error-00.js
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/error-01.js
--rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/error-02.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/01.js
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/02.js
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/03.js
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-00.js
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-01.js
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-02.js
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-03.js
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-04.js
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/01.js
--rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/02.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/03.js
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-00.js
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-01.js
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-02.js
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-03.js
--rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-04.js
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/generic/01.js
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/generic/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/generic/error-02.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/01.js
--rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/03.js
--rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-00.js
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-01.js
--rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-02.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-03.js
--rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-04.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/01.js
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/02.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/03.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/error-00.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/error-01.js
--rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/error-02.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/01.js
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/error-00.js
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/error-01.js
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/error-02.js
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/map/01.js
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/map/error-01.js
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mapbubble/01.js
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mapbubble/error-01.js
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mapline/01.js
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mapline/error-01.js
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mappoint/01.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/mappoint/error-01.js
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/01.js
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/error-00.js
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/error-01.js
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/error-02.js
--rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/01.js
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/error-00.js
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/error-01.js
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/error-02.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/01.js
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/error-00.js
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/error-01.js
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/error-02.js
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/01.js
--rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/02.js
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/03.js
--rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/04.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-00.js
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-01.js
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-02.js
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-03.js
--rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-04.js
--rw-r--r--   0        0        0   396839 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/plot_options/01.js
--rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/01.js
--rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/error-00.js
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/error-01.js
--rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/error-02.js
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/01.js
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/error-00.js
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/error-01.js
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/error-02.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/01.js
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/error-02.js
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/01.js
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/error-00.js
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/error-02.js
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/01.js
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/error-00.js
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/error-01.js
--rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/error-02.js
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/01.js
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/error-00.js
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/error-01.js
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/error-02.js
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/01.js
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/error-00.js
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/error-01.js
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/error-02.js
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/01.js
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/error-00.js
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/error-01.js
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/error-02.js
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/01.js
--rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/error-00.js
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/error-01.js
--rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/error-02.js
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/01.js
--rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/error-00.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/error-01.js
--rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/error-02.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/responsive/01.js
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/responsive/02.js
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/responsive/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/responsive/error-02.js
--rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/arcdiagram/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/arcdiagram/error-00.js
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/arcdiagram/error-01.js
--rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/01.js
--rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/02.js
--rw-r--r--   0        0        0    15908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/03.js
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/04.js
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/05.js
--rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/06.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-00.js
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-01.js
--rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-02.js
--rw-r--r--   0        0        0    16547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-03.js
--rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-04.js
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/01.js
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/02.js
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/03.js
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/04.js
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/05.js
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/06.js
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/07.js
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/08.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/error-00.js
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bar/error-01.js
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/01.js
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/02.js
--rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/03.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/error-00.js
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/error-01.js
--rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/base/error-02.js
--rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bellcurve/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bellcurve/error-00.js
--rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bellcurve/error-01.js
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/01.js
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/error-00.js
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/error-01.js
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/error-02.js
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bubble/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bubble/error-00.js
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bubble/error-01.js
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bullet/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bullet/error-00.js
--rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/bullet/error-01.js
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/01.js
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/02.js
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/03.js
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/04.js
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/05.js
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/06.js
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-01.js
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-02.js
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-03.js
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-04.js
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/base/01.js
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/base/error-01.js
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/boxplot/01.js
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/boxplot/error-01.js
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bullet/01.js
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/bullet/error-01.js
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/01.js
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/02.js
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/03.js
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/04.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/05.js
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/06.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/07.js
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/08.js
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-01.js
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-02.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-05.js
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-07.js
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/01.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/02.js
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/03.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/04.js
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-01.js
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-02.js
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-03.js
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/01.js
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/02.js
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/03.js
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/error-01.js
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/error-03.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/async_map_data/01-expected.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/async_map_data/01-input.js
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/01.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/02.js
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/03.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/error-01.js
--rw-r--r--   0        0        0   433034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/world.geo.json
--rw-r--r--   0        0        0   153391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/world.topo.json
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/01.js
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/02.js
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/error-01.js
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/error-02.js
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/01.js
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/02.js
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/03.js
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/04.js
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/error-01.js
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/error-02.js
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/error-03.js
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/01.js
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/02.js
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/03.js
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/04.js
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/05.js
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/06.js
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-01.js
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-02.js
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-03.js
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-04.js
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-05.js
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-06.js
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/01.js
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/02.js
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/error-01.js
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/error-02.js
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/vector/01.js
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/vector/error-01.js
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/venn/01.js
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/venn/error-01.js
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/wordcloud/01.js
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/data/wordcloud/error-01.js
--rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dependencywheel/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dependencywheel/error-00.js
--rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dependencywheel/error-01.js
--rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dumbbell/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dumbbell/error-00.js
--rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/dumbbell/error-01.js
--rw-r--r--   0        0        0     9240 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/01.js
--rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/error-00.js
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/error-01.js
--rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/error-02.js
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/01.js
--rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/error-00.js
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/error-01.js
--rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/error-02.js
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/generic/01.js
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/generic/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/generic/error-02.js
--rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/01.js
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/error-00.js
--rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/error-01.js
--rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/error-02.js
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/histogram/01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/histogram/error-00.js
--rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/histogram/error-01.js
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/item/01.js
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/item/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/item/error-00.js
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/item/error-01.js
--rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/item/error-02.js
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/map/01.js
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/map/error-01.js
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mapbubble/01.js
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mapbubble/error-01.js
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mapline/01.js
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mapline/error-01.js
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mappoint/01.js
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/mappoint/error-01.js
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/01.js
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/error-00.js
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/error-01.js
--rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/error-02.js
--rw-r--r--   0        0        0     9388 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/organization/01.js
--rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/organization/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/organization/error-00.js
--rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/organization/error-01.js
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/organization/error-02.js
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/01.js
--rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/error-00.js
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/error-01.js
--rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/error-02.js
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/01.js
--rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/02.js
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/error-01.js
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pie/01.js
--rw-r--r--   0        0        0     9268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pie/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pie/error-00.js
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pie/error-01.js
--rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/pie/error-02.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/01.js
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/02.js
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/error-01.js
--rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/error-02.js
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/01.js
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/error-00.js
--rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/error-01.js
--rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/error-02.js
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/01.js
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/error-00.js
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/error-01.js
--rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/error-02.js
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/spline/01.js
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/spline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/spline/error-00.js
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/spline/error-01.js
--rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/spline/error-02.js
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/01.js
--rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/error-00.js
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/error-01.js
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/error-02.js
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/01.js
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/error-00.js
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/error-01.js
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/error-02.js
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/01.js
--rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/error-00.js
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/error-01.js
--rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/error-02.js
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/vector/01.js
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/vector/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/vector/error-00.js
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/vector/error-01.js
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/vector/error-02.js
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/venn/01.js
--rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/venn/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/venn/error-00.js
--rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/venn/error-01.js
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/venn/error-02.js
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/01.js
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/02.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/error-00.js
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/error-01.js
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/error-02.js
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/subtitle/01.js
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/subtitle/02.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/subtitle/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/subtitle/error-02.js
--rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/test-data-files/nst-est2019-01-transposed.csv
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/test-data-files/nst-est2019-01.csv
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/time/01.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/time/02.js
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/time/error-01.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/time/error-02.js
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/title/01.js
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/title/02.js
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/title/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/title/error-02.js
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/tooltips/01.js
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/tooltips/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/tooltips/error-01.js
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/tooltips/error-02.js
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/animation/01.js
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/animation/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/animation/error-02.js
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/breadcrumbs/01.js
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/breadcrumbs/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/breadcrumbs/error-02.js
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/buttons/01.js
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/buttons/02.js
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/buttons/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/buttons/error-02.js
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/buttons/error-03.js
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/clusters/01.js
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/clusters/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/clusters/error-02.js
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_grouping/01.js
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_grouping/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_grouping/error-02.js
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/01.js
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/02.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/error-02.js
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/error-03.js
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/date_time_label_formats/01.js
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/date_time_label_formats/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/date_time_label_formats/error-02.js
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/01.js
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/02.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/03.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/04.js
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/05.js
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/06.js
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/07.js
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/08.js
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/09.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-00.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-01.js
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-02.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-03.js
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-04.js
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-05.js
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-06.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-07.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-08.js
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/events/error-09.js
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/gradients/01.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/gradients/02.js
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/gradients/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/gradients/error-02.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/gradients/error-03.js
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/jitter/01.js
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/jitter/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/jitter/error-02.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/markers/01.js
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/markers/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/markers/error-02.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/menus/01.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/menus/02.js
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/menus/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/menus/error-02.js
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/menus/error-03.js
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/01.js
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/02.js
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/03.js
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/error-02.js
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/error-03.js
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/nodes/error-04.js
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/partial_fill/01.js
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/partial_fill/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/partial_fill/error-02.js
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/patterns/01.js
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/patterns/02.js
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/patterns/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/patterns/error-02.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/patterns/error-03.js
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/position/01.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/position/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/position/error-02.js
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/shadows/01.js
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/shadows/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/shadows/error-02.js
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/states/01.js
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/states/02.js
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/states/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/states/error-02.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/zones/01.js
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/zones/02.js
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/zones/error-01.js
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/zones/error-02.js
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/zones/error-03.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/__init__.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_boost.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_caption.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_credits.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_data.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_defs.py
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_drilldown.py
--rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_loading.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_options.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_responsive.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_subtitle.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_time.py
--rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_title.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/test_tooltips.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/accessibility/__init__.py
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/accessibility/test_accessibility.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/annotations/__init__.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/annotations/test_annotation.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/__init__.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_color_axis.py
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_numeric.py
--rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_parallel_axes.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_plot_bands.py
--rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_x_axis.py
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_y_axis.py
--rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/axes/test_z_axis.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/chart/__init__.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/chart/test_chart.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/chart/test_options_3d.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/chart/test_zooming.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/exporting/__init__.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/exporting/test_csv.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/exporting/test_exporting.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/legend/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/legend/test_bubble_legend.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/legend/test_legend.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/legend/test_navigation.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/navigation/__init__.py
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/navigation/test_bindings.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/navigation/test_navigation.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/__init__.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_PlotOptions.py
--rw-r--r--   0        0        0    25301 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_arcdiagram.py
--rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_area.py
--rw-r--r--   0        0        0   141328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bar.py
--rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bellcurve.py
--rw-r--r--   0        0        0    37409 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_boxplot.py
--rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bubble.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bullet.py
--rw-r--r--   0        0        0    25444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_dependencywheel.py
--rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_dumbbell.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_funnel.py
--rw-r--r--   0        0        0    24453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_gauge.py
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_generic.py
--rw-r--r--   0        0        0    23344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_heatmap.py
--rw-r--r--   0        0        0    13615 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_histogram.py
--rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_item.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_map.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mapbubble.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mapline.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mappoint.py
--rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_networkgraph.py
--rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_organization.py
--rw-r--r--   0        0        0    12697 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_packedbubble.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pareto.py
--rw-r--r--   0        0        0    23106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pie.py
--rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_polygon.py
--rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pyramid.py
--rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_sankey.py
--rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_scatter.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_series.py
--rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_spline.py
--rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_sunburst.py
--rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_timeline.py
--rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_treemap.py
--rw-r--r--   0        0        0    27094 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_vector.py
--rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_venn.py
--rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/plot_options/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/__init__.py
--rw-r--r--   0        0        0    37684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_arcdiagram.py
--rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_area.py
--rw-r--r--   0        0        0   184797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_bar.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_base.py
--rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_bellcurve.py
--rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_boxplot.py
--rw-r--r--   0        0        0    27700 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_bubble.py
--rw-r--r--   0        0        0    19900 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_bullet.py
--rw-r--r--   0        0        0    38082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_dependencywheel.py
--rw-r--r--   0        0        0    25823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_dumbbell.py
--rw-r--r--   0        0        0    45949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_funnel.py
--rw-r--r--   0        0        0    43973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_gauge.py
--rw-r--r--   0        0        0    52024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_heatmap.py
--rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_histogram.py
--rw-r--r--   0        0        0    23439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_item.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_map.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_mapbubble.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_mapline.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_mappoint.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_networkgraph.py
--rw-r--r--   0        0        0    53769 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_organization.py
--rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_packedbubble.py
--rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_pareto.py
--rw-r--r--   0        0        0    42404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_pie.py
--rw-r--r--   0        0        0    26395 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_polygon.py
--rw-r--r--   0        0        0    45967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_pyramid.py
--rw-r--r--   0        0        0    38538 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_sankey.py
--rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_scatter.py
--rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_spline.py
--rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_sunburst.py
--rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_timeline.py
--rw-r--r--   0        0        0    23259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_treemap.py
--rw-r--r--   0        0        0    27497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_vector.py
--rw-r--r--   0        0        0    27155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_venn.py
--rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/__init__.py
--rw-r--r--   0        0        0    31572 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_bar.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_base.py
--rw-r--r--   0        0        0    22036 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_boxplot.py
--rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_bullet.py
--rw-r--r--   0        0        0    36534 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_cartesian.py
--rw-r--r--   0        0        0    30915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_connections.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_geometric.py
--rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_map_data.py
--rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_pie.py
--rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_range.py
--rw-r--r--   0        0        0    42349 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_single_point.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_sunburst.py
--rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_vector.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_venn.py
--rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/options/series/data/test_wordcloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_animation.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_ast.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_breadcrumbs.py
--rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_buttons.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_clusters.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_data_grouping.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_data_labels.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_date_time_label_formats.py
--rw-r--r--   0        0        0    21674 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_events.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_gradients.py
--rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_javascript_functions.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_jitter.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_markers.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_menus.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_nodes.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_partial_fill.py
--rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_patterns.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_position.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_shadows.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_states.py
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/tests/utility_classes/test_zones.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/.gitignore
--rw-r--r--   0        0        0    24468 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/LICENSE
--rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/README.rst
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.readthedocs.yaml
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.travis.yml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/CHANGES.rst
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.dev.txt
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.travis.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/requirements.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/setup.cfg
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tox.ini
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.github/workflows/pypi-test-publish.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/Makefile
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_contributors.rst
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_dependencies.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_installation.rst
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_support.rst
+-rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_versus_alternatives.rst
+-rw-r--r--   0        0        0    56205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api.rst
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/conf.py
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/contributing.rst
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/demos.rst
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/errors.rst
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/faq.rst
+-rw-r--r--   0        0        0    34457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/glossary.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/history.rst
+-rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/index.rst
+-rw-r--r--   0        0        0    24959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/license.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/links.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/make.bat
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/quickstart.rst
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/support.rst
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/testing.rst
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/toolkit.rst
+-rw-r--r--   0        0        0    38417 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using.rst
+-rw-r--r--   0        0        0    41670 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/visualizations.rst
+-rw-r--r--   0        0        0    54859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/abands-example.png
+-rw-r--r--   0        0        0    34552 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ad-example.png
+-rw-r--r--   0        0        0    43218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/apo-example.png
+-rw-r--r--   0        0        0    87899 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/arcdiagram-example.png
+-rw-r--r--   0        0        0    72487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/area-example.png
+-rw-r--r--   0        0        0   124371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/arearange-example.png
+-rw-r--r--   0        0        0    55288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/areaspline-example.png
+-rw-r--r--   0        0        0    54998 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/aroon-example.png
+-rw-r--r--   0        0        0    46438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/aroon-oscillator-example.png
+-rw-r--r--   0        0        0    47100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/atr-example.png
+-rw-r--r--   0        0        0    20359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/awesome-oscillator-example.png
+-rw-r--r--   0        0        0   485952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/axis-property-mapping.xlsx
+-rw-r--r--   0        0        0    59173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bar-example.png
+-rw-r--r--   0        0        0    48934 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bellcurve-example.png
+-rw-r--r--   0        0        0    43491 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bollinger-bands-example.png
+-rw-r--r--   0        0        0    37690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/boxplot-example.png
+-rw-r--r--   0        0        0    92954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bubble-example.png
+-rw-r--r--   0        0        0    26870 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/bullet-example.png
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/candlestick-example.png
+-rw-r--r--   0        0        0    52121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cci-example.png
+-rw-r--r--   0        0        0    49536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/chaikin-example.png
+-rw-r--r--   0        0        0    46772 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cmf-example.png
+-rw-r--r--   0        0        0    47632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cmo-example.png
+-rw-r--r--   0        0        0    41242 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/column-example.png
+-rw-r--r--   0        0        0    41567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked-horizontal.png
+-rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked.png
+-rw-r--r--   0        0        0    51790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example.png
+-rw-r--r--   0        0        0    63741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnrange-example-horizontal.png
+-rw-r--r--   0        0        0    68246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/columnrange-example.png
+-rw-r--r--   0        0        0    67368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/cylinder-example.png
+-rw-r--r--   0        0        0    54030 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dema-example.png
+-rw-r--r--   0        0        0   252801 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dependencywheel-example.png
+-rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/disparity-index-example.png
+-rw-r--r--   0        0        0    45925 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dmi-example.png
+-rw-r--r--   0        0        0    37726 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dpo-example.png
+-rw-r--r--   0        0        0    66693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/dumbbell-example.png
+-rw-r--r--   0        0        0    38446 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ema-example.png
+-rw-r--r--   0        0        0    59876 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/errorbar-example.png
+-rw-r--r--   0        0        0    27702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/flags-example.png
+-rw-r--r--   0        0        0    43626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/funnel-example.png
+-rw-r--r--   0        0        0    60815 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/funnel_3d-example.png
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/gantt-example.png
+-rw-r--r--   0        0        0   129516 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/gauge-example.png
+-rw-r--r--   0        0        0    87393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/heatmap-example.png
+-rw-r--r--   0        0        0    29731 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/heikin-ashi-example.png
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-dark-32x32.png
+-rw-r--r--   0        0        0     3746 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-light-150x149.png
+-rw-r--r--   0        0        0     9919 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-logo.svg
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/highcharts-python-logo.png
+-rw-r--r--   0        0        0    38747 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/histogram-example.png
+-rw-r--r--   0        0        0    25456 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/hlc-example.png
+-rw-r--r--   0        0        0    34397 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/hollow-candlestick-example.png
+-rw-r--r--   0        0        0    73793 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ikh-example.png
+-rw-r--r--   0        0        0   208287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-circular.png
+-rw-r--r--   0        0        0   151954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-rectangular.png
+-rw-r--r--   0        0        0    15447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/item-example-symbols.png
+-rw-r--r--   0        0        0    47093 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/keltner-channels-example.png
+-rw-r--r--   0        0        0    40750 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/klinger-example.png
+-rw-r--r--   0        0        0    81283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/line-example.png
+-rw-r--r--   0        0        0    59025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-angle-example.png
+-rw-r--r--   0        0        0    58305 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-example.png
+-rw-r--r--   0        0        0    54179 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-intercept-example.png
+-rw-r--r--   0        0        0    53628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/linear-regression-slope-example.png
+-rw-r--r--   0        0        0    47835 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/lollipop-example.png
+-rw-r--r--   0        0        0    41461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/macd-example.png
+-rw-r--r--   0        0        0   104539 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/map-example.png
+-rw-r--r--   0        0        0   201616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mapbubble-example.png
+-rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mapline-example.png
+-rw-r--r--   0        0        0   112234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mappoint-example.png
+-rw-r--r--   0        0        0    44732 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/mfi-example.png
+-rw-r--r--   0        0        0    51251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/momentum-example.png
+-rw-r--r--   0        0        0    49554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/natr-example.png
+-rw-r--r--   0        0        0    53945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/navigator-example.png
+-rw-r--r--   0        0        0   269275 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/networkgraph-example.png
+-rw-r--r--   0        0        0    34625 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/obv-example.png
+-rw-r--r--   0        0        0    34656 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ohlc-example.png
+-rw-r--r--   0        0        0    48433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/organization-example-horizontal.png
+-rw-r--r--   0        0        0   106952 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/organization-example.png
+-rw-r--r--   0        0        0   265002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example-split.png
+-rw-r--r--   0        0        0   298951 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example.png
+-rw-r--r--   0        0        0    58765 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pareto-example.png
+-rw-r--r--   0        0        0    90797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pie-example-donut.png
+-rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pie-example.png
+-rw-r--r--   0        0        0    47842 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pivot-points-example.png
+-rw-r--r--   0        0        0    56333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/polygon-example.png
+-rw-r--r--   0        0        0    44413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/ppo-example.png
+-rw-r--r--   0        0        0    55355 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/price-channel-example.png
+-rw-r--r--   0        0        0    43588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/price-envelopes-example.png
+-rw-r--r--   0        0        0    47048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/psar-example.png
+-rw-r--r--   0        0        0    49049 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pyramid-example.png
+-rw-r--r--   0        0        0    53531 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/pyramid_3d-example.png
+-rw-r--r--   0        0        0    44302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/range-selector-example.png
+-rw-r--r--   0        0        0    49944 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/roc-example.png
+-rw-r--r--   0        0        0    45958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/rsi-example.png
+-rw-r--r--   0        0        0   197682 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example-inverted.png
+-rw-r--r--   0        0        0    79510 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example-outgoing.png
+-rw-r--r--   0        0        0   227684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sankey-example.png
+-rw-r--r--   0        0        0   109494 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/scatter-example.png
+-rw-r--r--   0        0        0    29303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/scatter_3d-example.png
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/shared_options.js
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/shared_options_output.js
+-rw-r--r--   0        0        0    53177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/slow-stochastic-example.png
+-rw-r--r--   0        0        0    50549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sma-example.png
+-rw-r--r--   0        0        0    28628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/solidgauge-example.png
+-rw-r--r--   0        0        0     7807 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sphinx_rtd_theme_ext_color_contrast.css
+-rw-r--r--   0        0        0    81626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/spline-example.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/square-check-solid.svg
+-rw-r--r--   0        0        0    41933 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/stochastic-example.png
+-rw-r--r--   0        0        0    71303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/stock-tools-example.png
+-rw-r--r--   0        0        0   278653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/streamgraph-example.png
+-rw-r--r--   0        0        0   397432 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/sunburst-example.png
+-rw-r--r--   0        0        0    34040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/supertrend-example.png
+-rw-r--r--   0        0        0    55620 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tema-example.png
+-rw-r--r--   0        0        0   199024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-circle.png
+-rw-r--r--   0        0        0    95113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-diamond.png
+-rw-r--r--   0        0        0    81668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/tilemap-example.png
+-rw-r--r--   0        0        0    33235 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example-datetime.png
+-rw-r--r--   0        0        0    14778 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example-inverted.png
+-rw-r--r--   0        0        0    13386 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/timeline-example.png
+-rw-r--r--   0        0        0    59391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/treemap-example.png
+-rw-r--r--   0        0        0    44325 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/trendline-example.png
+-rw-r--r--   0        0        0    36104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/trix-example.png
+-rw-r--r--   0        0        0    64410 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variablepie-example.png
+-rw-r--r--   0        0        0    10175 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example-datetime.png
+-rw-r--r--   0        0        0    28517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example-inverted.png
+-rw-r--r--   0        0        0    74616 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/variwide-example.png
+-rw-r--r--   0        0        0    93945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vbp-example.png
+-rw-r--r--   0        0        0   173850 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vector-example.png
+-rw-r--r--   0        0        0    58194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/venn-example-euler.png
+-rw-r--r--   0        0        0    94796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/venn-example.png
+-rw-r--r--   0        0        0    41570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/vwap-example.png
+-rw-r--r--   0        0        0    59407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-inverted.png
+-rw-r--r--   0        0        0    12628 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-stacked.png
+-rw-r--r--   0        0        0    59664 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/waterfall-example.png
+-rw-r--r--   0        0        0    36821 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/williamsr-example.png
+-rw-r--r--   0        0        0    67964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/windbarb-example.png
+-rw-r--r--   0        0        0    52744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/wma-example.png
+-rw-r--r--   0        0        0   177320 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/wordcloud-example.png
+-rw-r--r--   0        0        0    28265 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/xrange-example-inverted.png
+-rw-r--r--   0        0        0    30421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/xrange-example.png
+-rw-r--r--   0        0        0    64223 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/_static/zigzag-example.png
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_class_structures.rst
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_deserialization_methods.rst
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_handling_defaults.rst
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_module_structure.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_other_convenience_methods.rst
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/_serialization_methods.rst
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/chart.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/headless_export.rst
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/highcharts.rst
+-rw-r--r--   0        0        0     7152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/internals.rst
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/index.rst
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/shared_options.rst
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/export_data.rst
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/index.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/navigation.rst
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/announce_new_data.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/axis.rst
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/chart_types.rst
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/exporting.rst
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/index.rst
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/legend.rst
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/range_selector.rst
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/screen_reader_section.rst
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/series.rst
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/sonification.rst
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/table.rst
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/zoom.rst
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/boost.rst
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/caption.rst
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/credits.rst
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/data.rst
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/defs.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/drilldown.rst
+-rw-r--r--   0        0        0    39926 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/index.rst
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/loading.rst
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_navigation.rst
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/responsive.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/subtitle.rst
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/time.rst
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/title.rst
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/tooltips.rst
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/announce_new_data.rst
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/index.rst
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/point.rst
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/screen_reader_section.rst
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/series.rst
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/focus_border.rst
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/index.rst
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/animation.rst
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/control_point_options.rst
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/events.rst
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/index.rst
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/label_options.rst
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/points.rst
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/annotations/shape_options.rst
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/accessibility.rst
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/breaks.rst
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/color_axis.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/crosshair.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/data_classes.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/generic.rst
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/index.rst
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/labels.rst
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/markers.rst
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/numeric.rst
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/parallel_axes.rst
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/plot_bands.rst
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/title.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/x_axis.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/y_axis.rst
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/axes/z_axis.rst
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/index.rst
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/options_3d.rst
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/reset_zoom_button.rst
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/scrollable_plot_area.rst
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/chart/zooming.rst
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/csv.rst
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/index.rst
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/exporting/pdf_font.rst
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/accessibility.rst
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/bubble_legend.rst
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/index.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/navigation.rst
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/legend/title.rst
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_views/index.rst
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/map_views/insets.rst
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/navigation/bindings.rst
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/navigation/index.rst
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/accessibility.rst
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/arcdiagram.rst
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/area.rst
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bar.rst
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/base.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bellcurve.rst
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/boxplot.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bubble.rst
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bullet.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/data_sorting.rst
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dependencywheel.rst
+-rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/drag_drop.rst
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dumbbell.rst
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/funnel.rst
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/gauge.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/generic.rst
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/heatmap.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/histogram.rst
+-rw-r--r--   0        0        0    13405 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/index.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/item.rst
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/levels.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/link.rst
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/map.rst
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapbubble.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapline.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mappoint.rst
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/networkgraph.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/organization.rst
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/packedbubble.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pareto.rst
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pie.rst
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/points.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/polygon.rst
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pyramid.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sankey.rst
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/scatter.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/series.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/spline.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sunburst.rst
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/timeline.rst
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/treemap.rst
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/vector.rst
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/venn.rst
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/plot_options/wordcloud.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/arcdiagram.rst
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/area.rst
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bar.rst
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/base.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bellcurve.rst
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/boxplot.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bubble.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/bullet.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/dependencywheel.rst
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/dumbbell.rst
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/funnel.rst
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/gauge.rst
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/heatmap.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/histogram.rst
+-rw-r--r--   0        0        0    13470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/index.rst
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/item.rst
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/labels.rst
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/map.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mapbubble.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mapline.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/mappoint.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/networkgraph.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/organization.rst
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/packedbubble.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pareto.rst
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pie.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/polygon.rst
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/pyramid.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/sankey.rst
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/scatter.rst
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/series_generator.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/spline.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/sunburst.rst
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/timeline.rst
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/treemap.rst
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/vector.rst
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/venn.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/wordcloud.rst
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/accessibility.rst
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/arcdiagram.rst
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/bar.rst
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/base.rst
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/boxplot.rst
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/bullet.rst
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/cartesian.rst
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/connections.rst
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/geometric.rst
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/index.rst
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/map_data.rst
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/pie.rst
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/range.rst
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/single_point.rst
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/sunburst.rst
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/treemap.rst
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/vector.rst
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/venn.rst
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/options/series/data/wordcloud.rst
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/animation.rst
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/ast.rst
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/breadcrumbs.rst
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/buttons.rst
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/clusters.rst
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_grouping.rst
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_labels.rst
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/date_time_label_formats.rst
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/events.rst
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/fetch_configuration.rst
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/geojson.rst
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/gradients.rst
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/index.rst
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/javascript_functions.rst
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/jitter.rst
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/markers.rst
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/menus.rst
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/nodes.rst
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/partial_fill.rst
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/patterns.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/position.rst
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/projections.rst
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/shadows.rst
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/states.rst
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/topojson.rst
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/api/utility_classes/zones.rst
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_code_style_naming_conventions.rst
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_importing.rst
+-rw-r--r--   0        0        0     7632 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/_working_with_maps_features.rst
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_add_series.rst
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_geopandas.rst
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_series.rst
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_series_property.rst
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_async_map_data.rst
+-rw-r--r--   0        0        0     7719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_synchronous_map_data.rst
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_chart_map.rst
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_series_map_data.rst
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_custom.rst
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_highsoft.rst
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_csv.rst
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_geopandas.rst
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pandas.rst
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pyspark.rst
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_csv.rst
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_geopandas.rst
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pandas.rst
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pyspark.rst
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_data_property.rst
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_from_array.rst
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_jupyter.rst
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_web_content.rst
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_dict.rst
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_js_literal.rst
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_json.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_copy.rst
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_dict.rst
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_js_literal.rst
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/docs/using/templates/_with_json.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/__version__.py
+-rw-r--r--   0        0        0    51211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/chart.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/constants.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/decorators.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/errors.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/headless_export.py
+-rw-r--r--   0        0        0     8075 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/highcharts.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/js_literal_functions.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/metaclasses.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/__init__.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/shared_options.py
+-rw-r--r--   0        0        0     4048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/__init__.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/export_data.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/navigation.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/announce_new_data.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/axis.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/chart_types.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/exporting.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/legend.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/range_selector.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/screen_reader_section.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/series.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/sonification.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/table.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/accessibility/zoom.py
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/boost.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/caption.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/credits.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/data.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/defs.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/drilldown.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/loading.py
+-rw-r--r--   0        0        0    11719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_navigation.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/responsive.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/subtitle.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/time.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/title.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/tooltips.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/announce_new_data.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/high_contrast_theme.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/point.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/screen_reader_section.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/series.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/focus_border.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/accessibility/keyboard_navigation/series_navigation.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/__init__.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/animation.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/control_point_options.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/events.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/label_options.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/points.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/annotations/shape_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/accessibility.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/breaks.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/color_axis.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/crosshair.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/data_classes.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/generic.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/labels.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/markers.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/numeric.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/parallel_axes.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/plot_bands.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/title.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/x_axis.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/y_axis.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/axes/z_axis.py
+-rw-r--r--   0        0        0    11458 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/__init__.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/options_3d.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/reset_zoom_button.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/scrollable_plot_area.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/zooming.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/csv.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/exporting/pdf_font.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/__init__.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/accessibility.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/bubble_legend.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/navigation.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/legend/title.py
+-rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/__init__.py
+-rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/insets.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/bindings.py
+-rw-r--r--   0        0        0    53247 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/accessibility.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/arcdiagram.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/area.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bar.py
+-rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bellcurve.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/boxplot.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bubble.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/bullet.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/data_sorting.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/dependencywheel.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/drag_drop.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/dumbbell.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/funnel.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/gauge.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/generic.py
+-rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/heatmap.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/histogram.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/item.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/levels.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/link.py
+-rw-r--r--   0        0        0    17236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/map.py
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapbubble.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapline.py
+-rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mappoint.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/networkgraph.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/organization.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/packedbubble.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pareto.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pie.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/points.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/polygon.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pyramid.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/sankey.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/scatter.py
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/series.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/spline.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/sunburst.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/timeline.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/treemap.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/vector.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/venn.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/arcdiagram.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/area.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bar.py
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/base.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bellcurve.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/boxplot.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bubble.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/bullet.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/dependencywheel.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/dumbbell.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/funnel.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/gauge.py
+-rw-r--r--   0        0        0    14416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/heatmap.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/histogram.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/item.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/labels.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/map.py
+-rw-r--r--   0        0        0     8470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapbubble.py
+-rw-r--r--   0        0        0     7162 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapline.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mappoint.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/networkgraph.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/organization.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/packedbubble.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pareto.py
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pie.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/polygon.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pyramid.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/sankey.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/scatter.py
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/series_generator.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/spline.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/sunburst.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/timeline.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/treemap.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/vector.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/venn.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/accessibility.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/arcdiagram.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/bar.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/base.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/boxplot.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/bullet.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/cartesian.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/connections.py
+-rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/geometric.py
+-rw-r--r--   0        0        0    26792 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/map_data.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/pie.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/range.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/single_point.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/sunburst.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/treemap.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/vector.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/venn.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/animation.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/ast.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/breadcrumbs.py
+-rw-r--r--   0        0        0     7047 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/buttons.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/clusters.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/data_grouping.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/data_labels.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/date_time_label_formats.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/events.py
+-rw-r--r--   0        0        0    14873 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/fetch_configuration.py
+-rw-r--r--   0        0        0    20197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/geojson.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/gradients.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/javascript_functions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/jitter.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/markers.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/menus.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/nodes.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/partial_fill.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/patterns.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/position.py
+-rw-r--r--   0        0        0    13187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/projections.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/shadows.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/states.py
+-rw-r--r--   0        0        0    23958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/topojson.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/zones.py
+-rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/__init__.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/conftest.py
+-rw-r--r--   0        0        0    37707 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/fixtures.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_chart.py
+-rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_decorators.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_headless_export.py
+-rw-r--r--   0        0        0     7798 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_js_literal_functions.py
+-rw-r--r--   0        0        0    10008 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_metaclasses.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_mro.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/test_utility_functions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/__init__.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/test_shared_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/__init__.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_export_data.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_language.py
+-rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/test_navigation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/__init__.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_accessibility.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_series.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/01.js
+-rw-r--r--   0        0        0     2125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-02.js
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/01.js
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-02.js
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/01.js
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/02.js
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/03.js
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/04.js
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/05.js
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/06.js
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/07.js
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/08.js
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/09.js
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/10.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-01.js
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-02.js
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-03.js
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-04.js
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-05.js
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-06.js
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-07.js
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-08.js
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-09.js
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-10.js
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/01.js
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/02.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-01.js
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-02.js
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/01.js
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/02.js
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-01.js
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-02.js
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/01.js
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/02.js
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-01.js
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-02.js
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/01.js
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/02.js
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-01.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-02.js
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/resize/01.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/resize/error-01.js
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/01.js
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/02.js
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-01.js
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-02.js
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/01.js
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/02.js
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-01.js
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-02.js
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/01.js
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/02.js
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-01.js
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-02.js
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/01.js
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/boost/error-02.js
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/01.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/02.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/caption/error-02.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/01.js
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-02.js
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/01.js
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-02.js
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/zooming/01.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart/zooming/error-01.js
+-rw-r--r--   0        0        0   461024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-expected.js
+-rw-r--r--   0        0        0   496450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-input.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/01.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/02.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/credits/error-02.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/01.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/02.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/data/error-02.js
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/01.js
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-02.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/01.js
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/csv/error-02.js
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/01.js
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-02.js
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/01.js
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-02.js
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/01.js
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/02.js
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-02.js
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-03.js
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/01.js
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/export_data/error-02.js
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/01.js
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-02.js
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/01.js
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/02.js
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-02.js
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-03.js
+-rw-r--r--   0        0        0   461353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-expected.js
+-rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-input.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/basic.json
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/with-chart-type.js
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/with-series-types.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/placeholder.txt
+-rw-r--r--   0        0        0    20068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-basic.png
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-chart-type.png
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/headless_export/output/test-with-series-types.png
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/01.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-02.js
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/01.js
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-02.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/01.js
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/legend/navigation/error-02.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/01.js
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/02.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/loading/error-02.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/01.js
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/02.js
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-02.js
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-03.js
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/01.js
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-02.js
+-rw-r--r--   0        0        0   461329 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/options/01.js
+-rw-r--r--   0        0        0     7103 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/01.js
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-02.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/01.js
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-00.js
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-01.js
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-02.js
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/01.js
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/02.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/03.js
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/04.js
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/05.js
+-rw-r--r--   0        0        0     6290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/06.js
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/07.js
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/08.js
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/09.js
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/10.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-02.js
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/01.js
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-00.js
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-01.js
+-rw-r--r--   0        0        0     7575 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-02.js
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/01.js
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-02.js
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/01.js
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-02.js
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/01.js
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-00.js
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-01.js
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-02.js
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/01.js
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-02.js
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/01.js
+-rw-r--r--   0        0        0     7490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-00.js
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-01.js
+-rw-r--r--   0        0        0     7503 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-02.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/01.js
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/02.js
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/03.js
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-00.js
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-01.js
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-02.js
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-03.js
+-rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-04.js
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/01.js
+-rw-r--r--   0        0        0     5851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/02.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/03.js
+-rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-00.js
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-01.js
+-rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-02.js
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-03.js
+-rw-r--r--   0        0        0     7333 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-04.js
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/01.js
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-02.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/01.js
+-rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/03.js
+-rw-r--r--   0        0        0     7363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-00.js
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-01.js
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-02.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-03.js
+-rw-r--r--   0        0        0     7368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-04.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/01.js
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/02.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/03.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-00.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-01.js
+-rw-r--r--   0        0        0     6295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-02.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/01.js
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-00.js
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-01.js
+-rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-02.js
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/map/01.js
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/map/error-01.js
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapbubble/01.js
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapbubble/error-01.js
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapline/01.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mapline/error-01.js
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mappoint/01.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/mappoint/error-01.js
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/01.js
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-00.js
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-01.js
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-02.js
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/01.js
+-rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-00.js
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-01.js
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-02.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/01.js
+-rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-00.js
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-01.js
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-02.js
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/01.js
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/02.js
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/03.js
+-rw-r--r--   0        0        0     6353 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/04.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-00.js
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-01.js
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-02.js
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-03.js
+-rw-r--r--   0        0        0     6363 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-04.js
+-rw-r--r--   0        0        0   396839 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/plot_options/01.js
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/01.js
+-rw-r--r--   0        0        0    11885 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-00.js
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-01.js
+-rw-r--r--   0        0        0    11810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-02.js
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/01.js
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-00.js
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-01.js
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-02.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/01.js
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-02.js
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/01.js
+-rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-00.js
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-02.js
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/01.js
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-00.js
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-01.js
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-02.js
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/01.js
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-00.js
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-01.js
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-02.js
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/01.js
+-rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-00.js
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-01.js
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-02.js
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/01.js
+-rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-00.js
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-01.js
+-rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-02.js
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/01.js
+-rw-r--r--   0        0        0     8895 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-00.js
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-01.js
+-rw-r--r--   0        0        0     8908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-02.js
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/01.js
+-rw-r--r--   0        0        0     5754 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-00.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-01.js
+-rw-r--r--   0        0        0     5767 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-02.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/01.js
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/02.js
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/responsive/error-02.js
+-rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-00.js
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-01.js
+-rw-r--r--   0        0        0     8346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/01.js
+-rw-r--r--   0        0        0     8662 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/02.js
+-rw-r--r--   0        0        0    15908 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/03.js
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/04.js
+-rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/05.js
+-rw-r--r--   0        0        0    13465 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/06.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-00.js
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-01.js
+-rw-r--r--   0        0        0     9285 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-02.js
+-rw-r--r--   0        0        0    16547 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-03.js
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-04.js
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/01.js
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/02.js
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/03.js
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/04.js
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/05.js
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/06.js
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/07.js
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/08.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-00.js
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-01.js
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/01.js
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/02.js
+-rw-r--r--   0        0        0     8833 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/03.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-00.js
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-01.js
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-02.js
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-00.js
+-rw-r--r--   0        0        0     7787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-01.js
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/01.js
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-00.js
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-01.js
+-rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-02.js
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-00.js
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-01.js
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-00.js
+-rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-01.js
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/01.js
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/02.js
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/03.js
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/04.js
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/05.js
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/06.js
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-01.js
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-02.js
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-03.js
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-04.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/01.js
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/error-01.js
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/01.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/error-01.js
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/01.js
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/error-01.js
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/01.js
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/02.js
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/03.js
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/04.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/05.js
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/06.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/07.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/08.js
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-01.js
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-02.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-05.js
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-07.js
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/01.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/02.js
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/03.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/04.js
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-01.js
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-02.js
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-03.js
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/01.js
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/02.js
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/03.js
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-01.js
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-03.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/async_map_data/01-expected.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/async_map_data/01-input.js
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/01.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/02.js
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/03.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/error-01.js
+-rw-r--r--   0        0        0   433034 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.geo.json
+-rw-r--r--   0        0        0   153391 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.topo.json
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/01.js
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/02.js
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-01.js
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-02.js
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/01.js
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/02.js
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/03.js
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/04.js
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-01.js
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-02.js
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-03.js
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/01.js
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/02.js
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/03.js
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/04.js
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/05.js
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/06.js
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-01.js
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-02.js
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-03.js
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-04.js
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-05.js
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-06.js
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/01.js
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/02.js
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-01.js
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-02.js
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/01.js
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/error-01.js
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/01.js
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/error-01.js
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/01.js
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/error-01.js
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-00.js
+-rw-r--r--   0        0        0    15237 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-01.js
+-rw-r--r--   0        0        0    10755 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-00.js
+-rw-r--r--   0        0        0    10775 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-01.js
+-rw-r--r--   0        0        0     9240 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/01.js
+-rw-r--r--   0        0        0     9266 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-00.js
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-01.js
+-rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-02.js
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/01.js
+-rw-r--r--   0        0        0    10204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-00.js
+-rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-01.js
+-rw-r--r--   0        0        0    10236 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-02.js
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/01.js
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-02.js
+-rw-r--r--   0        0        0     9920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/01.js
+-rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-00.js
+-rw-r--r--   0        0        0     9954 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-01.js
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-02.js
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-00.js
+-rw-r--r--   0        0        0     6313 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-01.js
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/01.js
+-rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-00.js
+-rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-01.js
+-rw-r--r--   0        0        0     9233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-02.js
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/map/01.js
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/map/error-01.js
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/01.js
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/error-01.js
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/01.js
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/error-01.js
+-rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/01.js
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/error-01.js
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/01.js
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-00.js
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-01.js
+-rw-r--r--   0        0        0     9403 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-02.js
+-rw-r--r--   0        0        0     9388 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/01.js
+-rw-r--r--   0        0        0    15633 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-00.js
+-rw-r--r--   0        0        0     9422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-01.js
+-rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-02.js
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/01.js
+-rw-r--r--   0        0        0     9528 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-00.js
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-01.js
+-rw-r--r--   0        0        0     9559 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-02.js
+-rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/01.js
+-rw-r--r--   0        0        0     7427 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/02.js
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/error-01.js
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/01.js
+-rw-r--r--   0        0        0     9268 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-00.js
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-01.js
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-02.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/01.js
+-rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/02.js
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-01.js
+-rw-r--r--   0        0        0    10431 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-02.js
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/01.js
+-rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-00.js
+-rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-01.js
+-rw-r--r--   0        0        0    15258 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-02.js
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/01.js
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-00.js
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-01.js
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-02.js
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/01.js
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-00.js
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-01.js
+-rw-r--r--   0        0        0     9785 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-02.js
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/01.js
+-rw-r--r--   0        0        0     9368 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-00.js
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-01.js
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-02.js
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/01.js
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-00.js
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-01.js
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-02.js
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/01.js
+-rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-00.js
+-rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-01.js
+-rw-r--r--   0        0        0    10359 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-02.js
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/01.js
+-rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-00.js
+-rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-01.js
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-02.js
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/01.js
+-rw-r--r--   0        0        0    11857 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-00.js
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-01.js
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-02.js
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/01.js
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/02.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-00.js
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-01.js
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-02.js
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/01.js
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/02.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/subtitle/error-02.js
+-rw-r--r--   0        0        0     7365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01-transposed.csv
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01.csv
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/01.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/02.js
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/error-01.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/time/error-02.js
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/01.js
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/02.js
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/title/error-02.js
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/01.js
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/error-01.js
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/tooltips/error-02.js
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/01.js
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/animation/error-02.js
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/01.js
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/breadcrumbs/error-02.js
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/01.js
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/02.js
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-02.js
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/buttons/error-03.js
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/01.js
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-02.js
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/01.js
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-02.js
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/01.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/02.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-02.js
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-03.js
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/01.js
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/date_time_label_formats/error-02.js
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/01.js
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/02.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/03.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/04.js
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/05.js
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/06.js
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/07.js
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/08.js
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/09.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-00.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-01.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-02.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-03.js
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-04.js
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-05.js
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-06.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-07.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-08.js
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/events/error-09.js
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/01.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/02.js
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-02.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/gradients/error-03.js
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/01.js
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/jitter/error-02.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/01.js
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/markers/error-02.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/01.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/02.js
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-02.js
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/menus/error-03.js
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/01.js
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/02.js
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/03.js
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-02.js
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-03.js
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/nodes/error-04.js
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/01.js
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/partial_fill/error-02.js
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/01.js
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/02.js
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-02.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/patterns/error-03.js
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/01.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/position/error-02.js
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/01.js
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/shadows/error-02.js
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/01.js
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/02.js
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/states/error-02.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/01.js
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/02.js
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-01.js
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-02.js
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/zones/error-03.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/__init__.py
+-rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_boost.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_caption.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_credits.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_data.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_defs.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_drilldown.py
+-rw-r--r--   0        0        0     2461 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_loading.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_options.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_responsive.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_subtitle.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_time.py
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_title.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/test_tooltips.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/accessibility/__init__.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/accessibility/test_accessibility.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/annotations/__init__.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/annotations/test_annotation.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/__init__.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_color_axis.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_numeric.py
+-rw-r--r--   0        0        0    12026 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_parallel_axes.py
+-rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_plot_bands.py
+-rw-r--r--   0        0        0     7249 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_x_axis.py
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_y_axis.py
+-rw-r--r--   0        0        0     7845 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/axes/test_z_axis.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/__init__.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_chart.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_options_3d.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/chart/test_zooming.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/__init__.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/test_csv.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/exporting/test_exporting.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_bubble_legend.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_legend.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/legend/test_navigation.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/__init__.py
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/test_bindings.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/navigation/test_navigation.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/__init__.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_PlotOptions.py
+-rw-r--r--   0        0        0    25301 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_arcdiagram.py
+-rw-r--r--   0        0        0    21498 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_area.py
+-rw-r--r--   0        0        0   141328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bar.py
+-rw-r--r--   0        0        0    12455 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bellcurve.py
+-rw-r--r--   0        0        0    37409 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_boxplot.py
+-rw-r--r--   0        0        0    14722 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bubble.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bullet.py
+-rw-r--r--   0        0        0    25444 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dependencywheel.py
+-rw-r--r--   0        0        0    14524 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dumbbell.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_funnel.py
+-rw-r--r--   0        0        0    24453 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_gauge.py
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_generic.py
+-rw-r--r--   0        0        0    23344 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_heatmap.py
+-rw-r--r--   0        0        0    13615 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_histogram.py
+-rw-r--r--   0        0        0    11791 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_item.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_map.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapbubble.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapline.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mappoint.py
+-rw-r--r--   0        0        0    11970 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_networkgraph.py
+-rw-r--r--   0        0        0    35312 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_organization.py
+-rw-r--r--   0        0        0    12697 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_packedbubble.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pareto.py
+-rw-r--r--   0        0        0    23106 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pie.py
+-rw-r--r--   0        0        0    13916 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_polygon.py
+-rw-r--r--   0        0        0    23521 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pyramid.py
+-rw-r--r--   0        0        0    25426 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sankey.py
+-rw-r--r--   0        0        0    16073 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_scatter.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_series.py
+-rw-r--r--   0        0        0    13914 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_spline.py
+-rw-r--r--   0        0        0    11946 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sunburst.py
+-rw-r--r--   0        0        0    11482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_timeline.py
+-rw-r--r--   0        0        0    14286 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_treemap.py
+-rw-r--r--   0        0        0    27094 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_vector.py
+-rw-r--r--   0        0        0    18068 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_venn.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/plot_options/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/__init__.py
+-rw-r--r--   0        0        0    37684 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_arcdiagram.py
+-rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_area.py
+-rw-r--r--   0        0        0   184797 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bar.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_base.py
+-rw-r--r--   0        0        0    11960 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bellcurve.py
+-rw-r--r--   0        0        0    38600 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_boxplot.py
+-rw-r--r--   0        0        0    27700 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bubble.py
+-rw-r--r--   0        0        0    19900 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_bullet.py
+-rw-r--r--   0        0        0    38082 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_dependencywheel.py
+-rw-r--r--   0        0        0    25823 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_dumbbell.py
+-rw-r--r--   0        0        0    45949 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_funnel.py
+-rw-r--r--   0        0        0    43973 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_gauge.py
+-rw-r--r--   0        0        0    52024 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_heatmap.py
+-rw-r--r--   0        0        0    13338 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_histogram.py
+-rw-r--r--   0        0        0    23439 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_item.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_map.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mapbubble.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mapline.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_mappoint.py
+-rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_networkgraph.py
+-rw-r--r--   0        0        0    53769 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_organization.py
+-rw-r--r--   0        0        0    27719 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_packedbubble.py
+-rw-r--r--   0        0        0    13693 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pareto.py
+-rw-r--r--   0        0        0    42404 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pie.py
+-rw-r--r--   0        0        0    26395 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_polygon.py
+-rw-r--r--   0        0        0    45967 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_pyramid.py
+-rw-r--r--   0        0        0    38538 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_sankey.py
+-rw-r--r--   0        0        0    29328 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_scatter.py
+-rw-r--r--   0        0        0    23877 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_spline.py
+-rw-r--r--   0        0        0    20920 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_sunburst.py
+-rw-r--r--   0        0        0    20357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_timeline.py
+-rw-r--r--   0        0        0    23259 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_treemap.py
+-rw-r--r--   0        0        0    27497 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_vector.py
+-rw-r--r--   0        0        0    27155 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_venn.py
+-rw-r--r--   0        0        0    18808 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/__init__.py
+-rw-r--r--   0        0        0    31572 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_bar.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_base.py
+-rw-r--r--   0        0        0    22036 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_boxplot.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_bullet.py
+-rw-r--r--   0        0        0    36534 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_cartesian.py
+-rw-r--r--   0        0        0    30915 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_connections.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_geometric.py
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_map_data.py
+-rw-r--r--   0        0        0    14300 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_pie.py
+-rw-r--r--   0        0        0    16010 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_range.py
+-rw-r--r--   0        0        0    42349 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_single_point.py
+-rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_sunburst.py
+-rw-r--r--   0        0        0    20702 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_vector.py
+-rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_venn.py
+-rw-r--r--   0        0        0     7102 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/options/series/data/test_wordcloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/__init__.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_animation.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_ast.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_breadcrumbs.py
+-rw-r--r--   0        0        0     7567 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_buttons.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_clusters.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_grouping.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_labels.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_date_time_label_formats.py
+-rw-r--r--   0        0        0    21674 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_events.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_gradients.py
+-rw-r--r--   0        0        0    17810 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_javascript_functions.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_jitter.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_markers.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_menus.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_nodes.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_partial_fill.py
+-rw-r--r--   0        0        0     4489 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_patterns.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_position.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_shadows.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_states.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/tests/utility_classes/test_zones.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/.gitignore
+-rw-r--r--   0        0        0    24468 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/LICENSE
+-rw-r--r--   0        0        0    17509 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/README.rst
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0    20818 2020-02-02 00:00:00.000000 highcharts_maps-1.0.0rc6/PKG-INFO
```

### Comparing `highcharts_maps-1.0.0rc5/.readthedocs.yaml` & `highcharts_maps-1.0.0rc6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/.travis.yml` & `highcharts_maps-1.0.0rc6/.travis.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/CODE_OF_CONDUCT.md` & `highcharts_maps-1.0.0rc6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tox.ini` & `highcharts_maps-1.0.0rc6/tox.ini`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/.github/ISSUE_TEMPLATE/bug_report.md` & `highcharts_maps-1.0.0rc6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/.github/workflows/pypi-publish.yml` & `highcharts_maps-1.0.0rc6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/.github/workflows/pypi-test-publish.yml` & `highcharts_maps-1.0.0rc6/.github/workflows/pypi-test-publish.yml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/Makefile` & `highcharts_maps-1.0.0rc6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_dependencies.rst` & `highcharts_maps-1.0.0rc6/docs/_dependencies.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_support.rst` & `highcharts_maps-1.0.0rc6/docs/_support.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_versus_alternatives.rst` & `highcharts_maps-1.0.0rc6/docs/_versus_alternatives.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api.rst` & `highcharts_maps-1.0.0rc6/docs/api.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/conf.py` & `highcharts_maps-1.0.0rc6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/contributing.rst` & `highcharts_maps-1.0.0rc6/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/errors.rst` & `highcharts_maps-1.0.0rc6/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/faq.rst` & `highcharts_maps-1.0.0rc6/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/glossary.rst` & `highcharts_maps-1.0.0rc6/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/index.rst` & `highcharts_maps-1.0.0rc6/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .. toctree::
   :hidden:
   :maxdepth: 3
   :caption: Contents
 
   Home <self>
   Quickstart: Patterns and Best Practices <quickstart>
+  Demos <demos>
   Supported Visualizations <visualizations>
   FAQ <faq>
   Toolkit Components and Roadmap <toolkit>
   Using Highcharts Maps for Python <using>
   API Reference <api>
   Error Reference <errors>
   Getting Help <support>
```

### Comparing `highcharts_maps-1.0.0rc5/docs/license.rst` & `highcharts_maps-1.0.0rc6/docs/license.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/make.bat` & `highcharts_maps-1.0.0rc6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/quickstart.rst` & `highcharts_maps-1.0.0rc6/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/toolkit.rst` & `highcharts_maps-1.0.0rc6/docs/toolkit.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using.rst` & `highcharts_maps-1.0.0rc6/docs/using.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/visualizations.rst` & `highcharts_maps-1.0.0rc6/docs/visualizations.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/abands-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/abands-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/ad-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/ad-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/apo-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/apo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/arcdiagram-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/arcdiagram-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/area-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/area-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/arearange-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/arearange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/areaspline-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/areaspline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/aroon-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/aroon-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/aroon-oscillator-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/aroon-oscillator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/atr-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/atr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/awesome-oscillator-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/awesome-oscillator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/axis-property-mapping.xlsx` & `highcharts_maps-1.0.0rc6/docs/_static/axis-property-mapping.xlsx`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/bar-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/bar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/bellcurve-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/bellcurve-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/bollinger-bands-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/bollinger-bands-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/boxplot-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/boxplot-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/bubble-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/bubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/bullet-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/bullet-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/candlestick-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/candlestick-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/cci-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/cci-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/chaikin-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/chaikin-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/cmf-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/cmf-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/cmo-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/cmo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/column-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/column-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example-stacked-horizontal.png` & `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example-stacked.png` & `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example-stacked.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/columnpyramid-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/columnpyramid-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/columnrange-example-horizontal.png` & `highcharts_maps-1.0.0rc6/docs/_static/columnrange-example-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/columnrange-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/columnrange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/cylinder-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/cylinder-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/dema-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/dema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/dependencywheel-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/dependencywheel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/disparity-index-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/disparity-index-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/dmi-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/dmi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/dpo-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/dpo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/dumbbell-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/dumbbell-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/ema-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/ema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/errorbar-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/errorbar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/flags-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/flags-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/funnel-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/funnel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/funnel_3d-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/funnel_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/gantt-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/gantt-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/gauge-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/gauge-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/heatmap-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/heatmap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/heikin-ashi-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/heikin-ashi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/highcharts-for-python-dark-32x32.png` & `highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-dark-32x32.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/highcharts-for-python-light-150x149.png` & `highcharts_maps-1.0.0rc6/docs/_static/highcharts-for-python-light-150x149.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/highcharts-logo.svg` & `highcharts_maps-1.0.0rc6/docs/_static/highcharts-logo.svg`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/highcharts-python-logo.png` & `highcharts_maps-1.0.0rc6/docs/_static/highcharts-python-logo.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/histogram-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/histogram-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/hlc-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/hlc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/hollow-candlestick-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/hollow-candlestick-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/ikh-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/ikh-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/item-example-circular.png` & `highcharts_maps-1.0.0rc6/docs/_static/item-example-circular.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/item-example-rectangular.png` & `highcharts_maps-1.0.0rc6/docs/_static/item-example-rectangular.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/item-example-symbols.png` & `highcharts_maps-1.0.0rc6/docs/_static/item-example-symbols.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/keltner-channels-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/keltner-channels-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/klinger-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/klinger-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/line-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/line-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/linear-regression-angle-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-angle-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/linear-regression-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/linear-regression-intercept-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-intercept-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/linear-regression-slope-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/linear-regression-slope-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/lollipop-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/lollipop-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/macd-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/macd-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/map-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/map-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/mapbubble-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/mapbubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/mapline-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/mapline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/mappoint-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/mappoint-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/mfi-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/mfi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/momentum-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/momentum-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/natr-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/natr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/navigator-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/navigator-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/networkgraph-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/networkgraph-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/obv-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/obv-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/ohlc-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/ohlc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/organization-example-horizontal.png` & `highcharts_maps-1.0.0rc6/docs/_static/organization-example-horizontal.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/organization-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/organization-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/packedbubble-example-split.png` & `highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example-split.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/packedbubble-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/packedbubble-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pareto-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/pareto-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pie-example-donut.png` & `highcharts_maps-1.0.0rc6/docs/_static/pie-example-donut.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pie-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/pie-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pivot-points-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/pivot-points-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/polygon-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/polygon-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/ppo-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/ppo-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/price-channel-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/price-channel-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/price-envelopes-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/price-envelopes-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/psar-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/psar-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pyramid-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/pyramid-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/pyramid_3d-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/pyramid_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/range-selector-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/range-selector-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/roc-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/roc-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/rsi-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/rsi-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sankey-example-inverted.png` & `highcharts_maps-1.0.0rc6/docs/_static/sankey-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sankey-example-outgoing.png` & `highcharts_maps-1.0.0rc6/docs/_static/sankey-example-outgoing.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sankey-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/sankey-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/scatter-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/scatter-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/scatter_3d-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/scatter_3d-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/shared_options.js` & `highcharts_maps-1.0.0rc6/docs/_static/shared_options.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/shared_options_output.js` & `highcharts_maps-1.0.0rc6/docs/_static/shared_options_output.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/slow-stochastic-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/slow-stochastic-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sma-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/sma-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/solidgauge-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/solidgauge-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sphinx_rtd_theme_ext_color_contrast.css` & `highcharts_maps-1.0.0rc6/docs/_static/sphinx_rtd_theme_ext_color_contrast.css`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/spline-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/spline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/stochastic-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/stochastic-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/stock-tools-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/stock-tools-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/streamgraph-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/streamgraph-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/sunburst-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/sunburst-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/supertrend-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/supertrend-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/tema-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/tema-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/tilemap-example-circle.png` & `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-circle.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/tilemap-example-diamond.png` & `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example-diamond.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/tilemap-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/tilemap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/timeline-example-datetime.png` & `highcharts_maps-1.0.0rc6/docs/_static/timeline-example-datetime.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/timeline-example-inverted.png` & `highcharts_maps-1.0.0rc6/docs/_static/timeline-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/timeline-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/timeline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/treemap-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/treemap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/trendline-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/trendline-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/trix-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/trix-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/variablepie-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/variablepie-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/variwide-example-datetime.png` & `highcharts_maps-1.0.0rc6/docs/_static/variwide-example-datetime.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/variwide-example-inverted.png` & `highcharts_maps-1.0.0rc6/docs/_static/variwide-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/variwide-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/variwide-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/vbp-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/vbp-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/vector-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/vector-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/venn-example-euler.png` & `highcharts_maps-1.0.0rc6/docs/_static/venn-example-euler.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/venn-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/venn-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/vwap-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/vwap-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/waterfall-example-inverted.png` & `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/waterfall-example-stacked.png` & `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example-stacked.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/waterfall-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/waterfall-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/williamsr-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/williamsr-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/windbarb-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/windbarb-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/wma-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/wma-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/wordcloud-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/wordcloud-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/xrange-example-inverted.png` & `highcharts_maps-1.0.0rc6/docs/_static/xrange-example-inverted.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/xrange-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/xrange-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/_static/zigzag-example.png` & `highcharts_maps-1.0.0rc6/docs/_static/zigzag-example.png`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_class_structures.rst` & `highcharts_maps-1.0.0rc6/docs/api/_class_structures.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_deserialization_methods.rst` & `highcharts_maps-1.0.0rc6/docs/api/_deserialization_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_handling_defaults.rst` & `highcharts_maps-1.0.0rc6/docs/api/_handling_defaults.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_module_structure.rst` & `highcharts_maps-1.0.0rc6/docs/api/_module_structure.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_other_convenience_methods.rst` & `highcharts_maps-1.0.0rc6/docs/api/_other_convenience_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/_serialization_methods.rst` & `highcharts_maps-1.0.0rc6/docs/api/_serialization_methods.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/chart.rst` & `highcharts_maps-1.0.0rc6/docs/api/chart.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/headless_export.rst` & `highcharts_maps-1.0.0rc6/docs/api/headless_export.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/highcharts.rst` & `highcharts_maps-1.0.0rc6/docs/api/highcharts.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/internals.rst` & `highcharts_maps-1.0.0rc6/docs/api/internals.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/shared_options.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/shared_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/export_data.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/export_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/navigation.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/announce_new_data.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/announce_new_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/axis.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/chart_types.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/chart_types.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/exporting.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/exporting.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/legend.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/legend.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/range_selector.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/range_selector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/screen_reader_section.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/screen_reader_section.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/series.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/sonification.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/sonification.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/table.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/table.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/global_options/language/accessibility/zoom.rst` & `highcharts_maps-1.0.0rc6/docs/api/global_options/language/accessibility/zoom.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/boost.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/boost.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/caption.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/caption.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/credits.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/credits.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/data.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/defs.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/defs.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/drilldown.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/drilldown.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/loading.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/loading.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/map_navigation.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/map_navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/responsive.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/responsive.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/subtitle.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/subtitle.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/time.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/time.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/title.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/tooltips.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/tooltips.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/announce_new_data.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/announce_new_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/point.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/point.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/screen_reader_section.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/screen_reader_section.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/series.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/focus_border.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/focus_border.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/accessibility/keyboard_navigation/series_navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/animation.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/animation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/control_point_options.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/control_point_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/events.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/events.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/label_options.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/label_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/points.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/points.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/annotations/shape_options.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/annotations/shape_options.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/accessibility.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/breaks.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/breaks.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/color_axis.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/color_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/crosshair.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/crosshair.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/data_classes.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/data_classes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/generic.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/generic.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/labels.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/markers.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/markers.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/numeric.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/numeric.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/parallel_axes.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/parallel_axes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/plot_bands.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/plot_bands.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/title.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/x_axis.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/x_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/y_axis.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/y_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/axes/z_axis.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/axes/z_axis.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/chart/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/chart/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/chart/options_3d.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/chart/options_3d.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/chart/reset_zoom_button.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/chart/reset_zoom_button.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/chart/scrollable_plot_area.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/chart/scrollable_plot_area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/chart/zooming.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/chart/zooming.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/exporting/csv.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/exporting/csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/exporting/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/exporting/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/exporting/pdf_font.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/exporting/pdf_font.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/legend/accessibility.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/legend/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/legend/bubble_legend.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/legend/bubble_legend.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/legend/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/legend/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/legend/navigation.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/legend/navigation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/legend/title.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/legend/title.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/map_views/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/map_views/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/map_views/insets.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/map_views/insets.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/navigation/bindings.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/navigation/bindings.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/navigation/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/navigation/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/accessibility.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/arcdiagram.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/area.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bar.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/base.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bellcurve.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bellcurve.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/boxplot.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/bullet.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/data_sorting.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/data_sorting.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/dependencywheel.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dependencywheel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/drag_drop.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/drag_drop.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/dumbbell.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/dumbbell.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/funnel.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/funnel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/gauge.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/gauge.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/generic.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/generic.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/heatmap.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/heatmap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/histogram.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/histogram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/item.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/item.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/levels.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/levels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/link.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/link.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/map.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mapbubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mapline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mapline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/mappoint.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/mappoint.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/networkgraph.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/networkgraph.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/organization.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/organization.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/packedbubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/packedbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pareto.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pareto.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pie.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/points.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/points.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/polygon.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/polygon.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/pyramid.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/pyramid.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/sankey.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sankey.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/scatter.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/scatter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/series.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/spline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/spline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/sunburst.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/timeline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/timeline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/treemap.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/vector.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/venn.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/plot_options/wordcloud.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/plot_options/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/arcdiagram.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/area.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/area.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/bar.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/base.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/bellcurve.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/bellcurve.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/boxplot.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/bubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/bubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/bullet.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/dependencywheel.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/dependencywheel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/dumbbell.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/dumbbell.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/funnel.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/funnel.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/gauge.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/gauge.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/heatmap.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/heatmap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/histogram.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/histogram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/item.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/item.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/labels.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/map.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/mapbubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/mapbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/mapline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/mapline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/mappoint.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/mappoint.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/networkgraph.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/networkgraph.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/organization.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/organization.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/packedbubble.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/packedbubble.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/pareto.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/pareto.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/pie.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/polygon.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/polygon.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/pyramid.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/pyramid.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/sankey.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/sankey.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/scatter.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/scatter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/series_generator.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/series_generator.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/spline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/spline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/sunburst.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/timeline.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/timeline.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/treemap.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/vector.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/venn.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/wordcloud.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/accessibility.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/accessibility.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/arcdiagram.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/arcdiagram.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/bar.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/bar.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/base.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/base.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/boxplot.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/boxplot.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/bullet.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/bullet.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/cartesian.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/cartesian.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/connections.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/connections.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/geometric.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/geometric.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/map_data.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/pie.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/pie.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/range.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/range.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/single_point.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/single_point.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/sunburst.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/sunburst.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/treemap.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/treemap.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/vector.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/vector.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/venn.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/venn.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/options/series/data/wordcloud.rst` & `highcharts_maps-1.0.0rc6/docs/api/options/series/data/wordcloud.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/animation.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/animation.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/ast.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/ast.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/breadcrumbs.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/buttons.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/buttons.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/clusters.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/clusters.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/data_grouping.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_grouping.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/data_labels.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/data_labels.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/date_time_label_formats.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/date_time_label_formats.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/events.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/events.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/fetch_configuration.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/fetch_configuration.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/geojson.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/geojson.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/gradients.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/gradients.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/index.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/index.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/javascript_functions.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/javascript_functions.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/jitter.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/jitter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/markers.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/markers.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/menus.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/menus.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/nodes.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/nodes.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/partial_fill.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/partial_fill.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/patterns.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/patterns.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/position.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/position.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/projections.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/projections.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/shadows.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/shadows.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/states.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/states.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/topojson.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/topojson.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/api/utility_classes/zones.rst` & `highcharts_maps-1.0.0rc6/docs/api/utility_classes/zones.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/_code_style_naming_conventions.rst` & `highcharts_maps-1.0.0rc6/docs/using/_code_style_naming_conventions.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/_importing.rst` & `highcharts_maps-1.0.0rc6/docs/using/_importing.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/_working_with_maps_features.rst` & `highcharts_maps-1.0.0rc6/docs/using/_working_with_maps_features.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_add_series.rst` & `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_add_series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_from_geopandas.rst` & `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_from_series.rst` & `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_from_series.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/assembling_your_chart/_using_series_property.rst` & `highcharts_maps-1.0.0rc6/docs/using/assembling_your_chart/_using_series_property.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_using_async_map_data.rst` & `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_async_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_using_synchronous_map_data.rst` & `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_using_synchronous_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_with_chart_map.rst` & `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_chart_map.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/configuring_map_data/_with_series_map_data.rst` & `highcharts_maps-1.0.0rc6/docs/using/configuring_map_data/_with_series_map_data.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/download_visualizations/_using_custom.rst` & `highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_custom.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/download_visualizations/_using_highsoft.rst` & `highcharts_maps-1.0.0rc6/docs/using/download_visualizations/_using_highsoft.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_csv.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_geopandas.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_pandas.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_load_from_pyspark.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_load_from_pyspark.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_csv.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_csv.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_geopandas.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_geopandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_pandas.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pandas.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_new_from_pyspark.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_new_from_pyspark.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_with_data_property.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_data_property.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/populating_series_data/_with_from_array.rst` & `highcharts_maps-1.0.0rc6/docs/using/populating_series_data/_with_from_array.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/rendering_your_visualizations/_as_jupyter.rst` & `highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_jupyter.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/rendering_your_visualizations/_as_web_content.rst` & `highcharts_maps-1.0.0rc6/docs/using/rendering_your_visualizations/_as_web_content.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_dict.rst` & `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_dict.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_js_literal.rst` & `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_js_literal.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/shared_options/_with_json.rst` & `highcharts_maps-1.0.0rc6/docs/using/shared_options/_with_json.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/templates/_with_copy.rst` & `highcharts_maps-1.0.0rc6/docs/using/templates/_with_copy.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/templates/_with_js_literal.rst` & `highcharts_maps-1.0.0rc6/docs/using/templates/_with_js_literal.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/docs/using/templates/_with_json.rst` & `highcharts_maps-1.0.0rc6/docs/using/templates/_with_json.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/chart.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,53 +58,63 @@
                 js_str += """});"""
 
         return js_str
 
     def _jupyter_javascript(self, 
                             global_options = None, 
                             container = None,
+                            random_slug = None,
                             retries = 3,
                             interval = 1000):
         """Return the JavaScript code which Jupyter Labs will need to render the chart.
 
         :param global_options: The :term:`shared options` to use when rendering the chart.
           Defaults to :obj:`None <python:None>`
         :type global_options: :class:`SharedOptions <highcharts_stock.global_options.shared_options.SharedOptions>`
           or :obj:`None <python:None>`
           
         :param container: The ID to apply to the HTML container when rendered in Jupyter Labs. Defaults to
           :obj:`None <python:None>`, which applies the :meth:`.container <highcharts_core.chart.Chart.container>` 
           property if set, and ``'highcharts_target_div'`` if not set.
         :type container: :class:`str <python:str>` or :obj:`None <python:None>`
 
+        :param random_slug: The random sequence of characters to append to the container name to ensure uniqueness.
+          Defaults to :obj:`None <python:None>`
+        :type random_slug: :class:`str <python:str>` or :obj:`None <python:None>`
+        
         :param retries: The number of times to retry rendering the chart. Used to avoid race conditions with the 
           Highcharts script. Defaults to 3.
         :type retries: :class:`int <python:int>`
         
         :param interval: The number of milliseconds to wait between retrying rendering the chart. Defaults to 1000 (1 
           seocnd).
         :type interval: :class:`int <python:int>`
 
         :rtype: :class:`str <python:str>`
         """
         original_container = self.container
-        self.container = container or self.container or 'highcharts_target_div'
+        new_container = container or self.container or 'highcharts_target_div'
+        if not random_slug:
+            self.container = new_container
+        else:
+            self.container = f'{new_container}_{random_slug}'
         
         if global_options is not None:
             global_options = validate_types(global_options,
                                             types = (SharedMapsOptions, SharedOptions))
 
         js_str = ''
         js_str += utility_functions.get_retryHighcharts()
 
         if global_options:
             js_str += '\n' + utility_functions.prep_js_for_jupyter(global_options.to_js_literal()) + '\n'
 
         js_str += utility_functions.prep_js_for_jupyter(self.to_js_literal(),
                                                         container = self.container,
+                                                        random_slug = random_slug,
                                                         retries = retries,
                                                         interval = interval)
 
         self.container = original_container
 
         return js_str
 
@@ -250,15 +260,20 @@
         else:
             container_as_str = """null"""
         signature_elements += 1
 
         options_as_str = ''
         if self.options:
             options_as_str = self.options.to_js_literal(encoding = encoding)
-            if self.options.chart and self.options.chart.map and self.options.chart.is_async:
+            if (
+                self.is_maps_chart and 
+                hasattr(self.options.chart, 'map') and 
+                self.options.chart.map and 
+                self.options.chart.is_async
+            ):
                 chart_map_str = self.options.chart.map.to_js_literal(encoding = encoding)
                 chart_map_str = f"""'{chart_map_str}'"""
                 fetch_counter = self.options.chart.map.fetch_counter
                 options_as_str = options_as_str.replace(chart_map_str, f'topology{fetch_counter}')
             options_as_str = f"""{options_as_str}"""
         else:
             options_as_str = """{}"""
@@ -451,46 +466,14 @@
         :rtype: :class:`Chart <highcharts_maps.chart.Chart>`
         """
         kwargs = validators.dict(kwargs, allow_empty = True) or {}
         instance = cls(**kwargs)
 
         instance.add_series(series)
 
-    def display(self, global_options = None):
-        """Display the chart in `Jupyter Labs <https://jupyter.org/>`_ or
-        `Jupyter Notebooks <https://jupyter.org/>`_.
-
-        :raises HighchartsDependencyError: if
-          `ipython <https://ipython.readthedocs.io/en/stable/>`_ is not available in the
-          runtime environment
-        """
-        try:
-            from IPython import display
-        except ImportError:
-            raise errors.HighchartsDependencyError('Unable to import IPython.display. '
-                                                   'Make sure that it is available in '
-                                                   'your runtime environment. To install,'
-                                                   'use: pip install ipython')
-
-        if global_options is not None:
-            global_options = validate_types(global_options,
-                                            types = SharedMapsOptions)
-
-        if self.is_maps_chart:
-            include_str = constants.MAPS_INCLUDE_STR
-        else:
-            include_str = constants.INCLUDE_STR
-
-        html_str = include_str + '\n'
-        if global_options:
-            html_str += global_options._repr_html_() + '\n'
-        html_str += self._repr_html_()
-
-        display.display_html(html_str, raw = True)
-
     @staticmethod
     def _get_options_obj(series_type, options_kwargs):
         """Return an :class:`Options` descendent based on the series type.
 
         :param series_type: Indicates the series type that should be created from the CSV
           data.
         :type series_type: :class:`str <python:str>`
@@ -1049,15 +1032,15 @@
           :class:`AsyncMapData <highcharts_maps.options.series.data.map_data.AsyncMapData>`
 
         :rtype: :class:`bool <python:bool>`
         """
         if not self.options or not self.options.series:
             return False
 
-        if self.options.chart and self.options.chart.is_async:
+        if self.options.chart and hasattr(self.options.chart, 'is_async') and self.options.chart.is_async:
             return True
 
         for series in self.options.series:
             if hasattr(series, 'is_async') and series.is_async:
                 return True
 
         return False
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/headless_export.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/headless_export.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/highcharts.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/highcharts.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_functions.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 from validator_collection import validators
 
 from highcharts_core.utility_functions import *
 
 from highcharts_maps import errors
 
+def to_snake_case(camelCase):
+    """Convert ``camelCase`` to ``snake_case``.
+    
+    :param camelCase: A :class:`str <python:str>` which is likely to contain
+      ``camelCase``.
+    :type camelCase: :class:`str <python:str>`
+
+    :returns: A ``snake_case`` representation of ``camel_case``.
+    :rtype: :class:`str <python:str>`
+    """
+    camelCase = validators.string(camelCase)
+    if '_' in camelCase:
+        return camelCase
+    
+    snake_case = ''
+    for character in camelCase:
+        if character.isupper():
+            snake_case += '_'
+        snake_case += character
+        
+    snake_case = snake_case.lower()
+    
+    return snake_case
+
+
 def validate_bounding_array(value,
                             allow_singleton = True,
                             allow_percentage_strings = True,
                             allow_numbers = True):
     """Validates that ``value`` is either a single value or a 4-member collection.
 
     :param value: The value to validate.
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/global_options/shared_options.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/global_options/shared_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/global_options/language/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/global_options/language/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/map_navigation.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/chart/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/chart/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from highcharts_maps.decorators import class_sensitive, validate_types
 from highcharts_maps.utility_classes.javascript_functions import (CallbackFunction,
                                                                   VariableName)
 
 from highcharts_maps.options.series.data.map_data import MapData, AsyncMapData
 
 from highcharts_core.options.chart import (PanningOptions,
-                                             ChartOptions as ChartOptionsBase)
+                                           ChartOptions as ChartOptionsBase)
 
 
 class ChartOptions(ChartOptionsBase):
     """Configuration settings that apply to a chart."""
 
     def __init__(self, **kwargs):
         self._map = None
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/map_views/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/map_views/insets.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/map_views/insets.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/navigation/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/navigation/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/__init__.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/base.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Optional, List
+from collections import UserDict
 
 from validator_collection import validators, checkers
 
 from highcharts_maps import constants, errors
 from highcharts_maps.options.plot_options.generic import HighchartsMeta
 
 
@@ -75,23 +76,26 @@
 
     @join_by.setter
     def join_by(self, value):
         if value is None:
             self._join_by = None
         elif isinstance(value, constants.EnforcedNullType):
             self._join_by = constants.EnforcedNull
-        elif checkers.is_iterable(value):
+        elif checkers.is_iterable(value, forbid_literals = (str, bytes, dict, UserDict)):
             if len(value) > 2:
                 raise errors.HighchartsValueError(f'join_by expects a 2-member iterable.'
                                                   f'Received a {len(value)}-member '
                                                   f'iterable.')
             elif len(value) == 2:
-                self._join_by = validators.string(value[0])
+                self._join_by = [
+                    validators.string(value[0]),
+                    validators.string(value[1])
+                ]
             else:
-                self._join_by = [validators.string(x) for x in value]
+                self._join_by = validators.string(value)
         else:
             self._join_by = validators.string(value)
 
     @classmethod
     def _get_kwargs_from_dict(cls, as_dict):
         kwargs = {
             'all_areas': as_dict.get('allAreas', None),
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/heatmap.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/map.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mapbubble.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mapline.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/mappoint.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/pie.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/plot_options/series.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/plot_options/series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/base.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/heatmap.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/map.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mapbubble.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mapline.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/mappoint.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/pie.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/series_generator.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/series_generator.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/geometric.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/geometric.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,63 @@
-from typing import Optional
+from typing import Optional, List
 from decimal import Decimal
 
 from validator_collection import validators, checkers
 
-from highcharts_maps import constants, errors
-from highcharts_maps.decorators import class_sensitive
+from highcharts_maps import constants, errors, utility_functions
+from highcharts_maps.decorators import class_sensitive, validate_types
 from highcharts_maps.options.series.data.base import DataCore
 from highcharts_maps.utility_classes.data_labels import DataLabel
 from highcharts_maps.utility_classes.geojson import Feature
 
 
 class GeometricDataBase(DataCore):
     """Base class for representing geometric data on map charts."""
 
     def __init__(self, **kwargs):
         self._data_labels = None
         self._drilldown = None
         self._geometry = None
+        self._properties = None
+
         self.data_labels = kwargs.get('data_labels', None)
         self.drilldown = kwargs.get('drilldown', None)
         self.geometry = kwargs.get('geometry', None)
+        self.properties = kwargs.get('properties', None)
 
         super().__init__(**kwargs)
 
     @property
-    def data_labels(self) -> Optional[DataLabel]:
+    def data_labels(self) -> Optional[DataLabel | List[DataLabel]]:
         """Individual data label for the data point.
 
-        :rtype: :class:`DataLabel` or :obj:`None <python:None>`
+        .. note::
+
+          To have multiple data labels per data point, you can also supply a collection of
+          :class:`DataLabel` configuration settings.
+
+        :rtype: :class:`DataLabel`, :class:`list <python:list>` of :class:`DataLabel`, or
+          :obj:`None <python:None>`
         """
         return self._data_labels
 
     @data_labels.setter
-    @class_sensitive(DataLabel)
     def data_labels(self, value):
-        self._data_labels = value
+        if not value:
+            self._data_labels = None
+        else:
+            if checkers.is_iterable(value):
+                self._data_labels = validate_types(value,
+                                                   types = DataLabel,
+                                                   allow_none = False,
+                                                   force_iterable = True)
+            else:
+                self._data_labels = validate_types(value,
+                                                   types = DataLabel,
+                                                   allow_none = False)
 
     @property
     def drilldown(self) -> Optional[str]:
         """The :meth:`id <SeriesBase.id>` of a series in the ``drilldown.series`` array
         to use as a drilldown destination for this point. Defaults to
         :obj:`None <python:None>`.
 
@@ -73,14 +92,26 @@
         return self._geometry
 
     @geometry.setter
     @class_sensitive(Feature)
     def geometry(self, value):
         self._geometry = value
 
+    @property
+    def properties(self) -> Optional[dict]:
+        """Collection of properties associated with the geometric data point.
+        
+        :rtype: :class:`dict <python:dict>` or :obj:`None <python:None>`
+        """
+        return self._properties
+    
+    @properties.setter
+    def properties(self, value):
+        self._properties = validators.dict(value, allow_empty = True)
+
     @classmethod
     def _get_kwargs_from_dict(cls, as_dict):
         """Convenience method which returns the keyword arguments used to initialize the
         class from a Highcharts Javascript-compatible :class:`dict <python:dict>` object.
 
         :param as_dict: The HighCharts JS compatible :class:`dict <python:dict>`
           representation of the object.
@@ -107,22 +138,35 @@
 
             'data_labels': as_dict.get('dataLabels', None),
             'drag_drop': as_dict.get('dragDrop', None),
             'drilldown': as_dict.get('drilldown', None),
             'geometry': as_dict.get('geometry', None),
         }
 
+        properties = {}
+        if len(as_dict) > len(kwargs):
+            for key in as_dict:
+                if key not in kwargs:
+                    snake_key = utility_functions.to_snake_case(key)
+                    if snake_key not in kwargs:
+                        properties[snake_key] = as_dict[key]
+
+        kwargs['properties'] = properties
+
         return kwargs
 
     def _to_untrimmed_dict(self, in_cls = None) -> dict:
         untrimmed = {
             'dataLabels': self.data_labels,
             'drilldown': self.drilldown,
             'geometry': self.geometry,
         }
+        if self.properties:
+            for key in self.properties:
+                untrimmed[key] = self.properties[key]
 
         parent_as_dict = super()._to_untrimmed_dict(in_cls = in_cls)
         for key in parent_as_dict:
             untrimmed[key] = parent_as_dict[key]
 
         return untrimmed
 
@@ -296,14 +340,24 @@
 
             'middle_x': as_dict.get('middleX', None),
             'middle_y': as_dict.get('middleY', None),
             'path': as_dict.get('path', None),
             'value': as_dict.get('value', None),
         }
 
+        properties = {}
+        if len(as_dict) > len(kwargs):
+            for key in as_dict:
+                if key not in kwargs:
+                    snake_key = utility_functions.to_snake_case(key)
+                    if snake_key not in kwargs:
+                        properties[snake_key] = as_dict[key]
+                
+        kwargs['properties'] = properties
+
         return kwargs
 
     def _to_untrimmed_dict(self, in_cls = None) -> dict:
         untrimmed = {
             'middleX': self.middle_x,
             'middleY': self.middle_y,
             'path': self.path,
@@ -414,14 +468,24 @@
             'data_labels': as_dict.get('dataLabels', None),
             'drag_drop': as_dict.get('dragDrop', None),
             'drilldown': as_dict.get('drilldown', None),
             'geometry': as_dict.get('geometry', None),
             'z': as_dict.get('z', None),
         }
 
+        properties = {}
+        if len(as_dict) > len(kwargs):
+            for key in as_dict:
+                if key not in kwargs:
+                    snake_key = utility_functions.to_snake_case(key)
+                    if snake_key not in kwargs:
+                        properties[snake_key] = as_dict[key]
+                
+        kwargs['properties'] = properties
+
         return kwargs
 
     def _to_untrimmed_dict(self, in_cls = None) -> dict:
         untrimmed = {
             'z': self.z
         }
 
@@ -601,14 +665,24 @@
             'geometry': as_dict.get('geometry', None),
             'lat': as_dict.get('lat', None),
             'lon': as_dict.get('lon', None),
             'x': as_dict.get('x', None),
             'y': as_dict.get('y', None),
         }
 
+        properties = {}
+        if len(as_dict) > len(kwargs):
+            for key in as_dict:
+                if key not in kwargs:
+                    snake_key = utility_functions.to_snake_case(key)
+                    if snake_key not in kwargs:
+                        properties[snake_key] = as_dict[key]
+                
+        kwargs['properties'] = properties
+
         return kwargs
 
     def _to_untrimmed_dict(self, in_cls = None) -> dict:
         untrimmed = {
             'lat': self.lat,
             'lon': self.lon,
             'x': self.x,
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/options/series/data/map_data.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/options/series/data/map_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,16 +241,15 @@
         """
         if filename:
             filename = validators.path(filename)
 
         if not self.force_geojson:
             as_json = self.topology.to_json()
         else:
-            as_geojson = self.topology.to_geojson()
-            as_json = geojson.dumps(as_geojson)
+            as_json = self.topology.to_geojson()
 
         if filename:
             if isinstance(as_json, bytes):
                 write_type = 'wb'
             else:
                 write_type = 'w'
 
@@ -303,21 +302,26 @@
         :type encoding: :class:`str <python:str>`
 
         :rtype: :class:`str <python:str>` or :obj:`None <python:None>`
         """
         if filename:
             filename = validators.path(filename)
 
-        as_str = self.to_json(encoding = encoding)
+        as_json = self.to_json(encoding = encoding)
 
         if filename:
-            with open(filename, 'w', encoding = encoding) as file_:
-                file_.write(as_str)
+            if isinstance(as_json, bytes):
+                write_type = 'wb'
+            else:
+                write_type = 'w'
 
-        return as_str
+            with open(filename, write_type, encoding = encoding) as file_:
+                file_.write(as_json)
+
+        return as_json
 
     def to_geojson(self,
                    filename = None,
                    encoding = 'utf-8'):
         """Generate a :term:`GeoJSON` string/byte string representation of the object.
 
         .. note::
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/buttons.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/buttons.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/fetch_configuration.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/fetch_configuration.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/geojson.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/geojson.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/projections.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/projections.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,16 @@
         """
         return self._custom
 
     @custom.setter
     @class_sensitive(CustomProjection)
     def custom(self, value):
         self._custom = value
-        self.name = self.custom.name
+        if value is not None:
+            self.name = self.custom.name
 
     @classmethod
     def _get_kwargs_from_dict(cls, as_dict):
         kwargs = {
             'name': as_dict.get('name', None),
             'parallels': as_dict.get('parallels', None),
             'rotation': as_dict.get('rotation', None),
```

### Comparing `highcharts_maps-1.0.0rc5/highcharts_maps/utility_classes/topojson.py` & `highcharts_maps-1.0.0rc6/highcharts_maps/utility_classes/topojson.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/__init__.py` & `highcharts_maps-1.0.0rc6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/conftest.py` & `highcharts_maps-1.0.0rc6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/fixtures.py` & `highcharts_maps-1.0.0rc6/tests/fixtures.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,16 +297,16 @@
     if not isinstance(original, str):
         original = str(original)
     if not isinstance(new, str):
         new = str(new)
 
     counter = 0
     for char in original:
-        min_index = max(0, counter - 20)
-        max_index = min(counter + 20, len(original))
+        min_index = max(0, counter - 200)
+        max_index = min(counter + 200, len(original))
 
         if new[counter] != char:
             print(f'\nMISMATCH FOUND AT ORIGINAL CHARACTER: {counter}')
             print(f'-- ORIGINAL: {original[min_index:max_index]}\n\n')
             print(f'-- NEW: {new[min_index:max_index]}')
 
             original_fragment = original[min_index:max_index].strip()
```

### Comparing `highcharts_maps-1.0.0rc5/tests/test_chart.py` & `highcharts_maps-1.0.0rc6/tests/test_chart.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/test_decorators.py` & `highcharts_maps-1.0.0rc6/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/test_headless_export.py` & `highcharts_maps-1.0.0rc6/tests/test_headless_export.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/test_js_literal_functions.py` & `highcharts_maps-1.0.0rc6/tests/test_js_literal_functions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/test_metaclasses.py` & `highcharts_maps-1.0.0rc6/tests/test_metaclasses.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/test_mro.py` & `highcharts_maps-1.0.0rc6/tests/test_mro.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/test_shared_options.py` & `highcharts_maps-1.0.0rc6/tests/global_options/test_shared_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/language/test_export_data.py` & `highcharts_maps-1.0.0rc6/tests/global_options/language/test_export_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/language/test_language.py` & `highcharts_maps-1.0.0rc6/tests/global_options/language/test_language.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/language/test_navigation.py` & `highcharts_maps-1.0.0rc6/tests/global_options/language/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/language/accessibility/test_accessibility.py` & `highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_accessibility.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/global_options/language/accessibility/test_series.py` & `highcharts_maps-1.0.0rc6/tests/global_options/language/accessibility/test_series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/accessibility/accessibility/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/accessibility/accessibility/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/accessibility/accessibility/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/annotation/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/annotation/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/annotation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/07.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/08.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/09.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/10.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-07.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-08.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-09.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/annotations/stock_tools/error-10.js` & `highcharts_maps-1.0.0rc6/tests/input_files/annotations/stock_tools/error-10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/color_axis/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/color_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/numeric/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/numeric/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/parallel_axes/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/parallel_axes/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/plot_bands/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/plot_bands/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/x_axis/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/x_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/y_axis/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/y_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/axes/z_axis/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/axes/z_axis/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart/chart/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart/chart/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart/chart/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart/options_3d/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart/options_3d/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart/options_3d/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart_obj/01-expected.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-expected.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/chart_obj/01-input.js` & `highcharts_maps-1.0.0rc6/tests/input_files/chart_obj/01-input.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/drilldown/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/drilldown/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/drilldown/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/drilldown/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/exporting/exporting/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/exporting/exporting/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/exporting/exporting/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/accessibility/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/accessibility/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/accessibility/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/accessibility/series/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/accessibility/series/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/language/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/language/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/language/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/language/navigation/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/language/navigation/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/shared_options/01-expected.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-expected.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/global_options/shared_options/01-input.js` & `highcharts_maps-1.0.0rc6/tests/input_files/global_options/shared_options/01-input.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/legend/bubble_legend/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/legend/bubble_legend/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/legend/bubble_legend/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/legend/legend/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/legend/legend/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/legend/legend/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/navigation/bindings/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/navigation/bindings/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/navigation/navigation/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/navigation/navigation/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/options/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/options/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/arcdiagram/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/arcdiagram/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/area/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/area/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/07.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/08.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/09.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/09.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/10.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/10.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bar/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bar/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bellcurve/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bellcurve/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/boxplot/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/boxplot/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bubble/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/bullet/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/bullet/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dependencywheel/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dependencywheel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/dumbbell/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/dumbbell/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/funnel/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/funnel/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/gauge/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/gauge/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/generic/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/generic/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/generic/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/heatmap/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/heatmap/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/histogram/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/histogram/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/item/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/item/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/networkgraph/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/networkgraph/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/organization/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/organization/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/packedbubble/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/packedbubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/pie/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/pie/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/plot_options/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/plot_options/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sankey/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sankey/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/scatter/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/scatter/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/series/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/series/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/spline/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/spline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/sunburst/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/timeline/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/timeline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/treemap/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/treemap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/vector/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/vector/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/venn/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/venn/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/plot_options/wordcloud/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/plot_options/wordcloud/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/arcdiagram/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/arcdiagram/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/arcdiagram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/area/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/area/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/07.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/07.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/08.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bar/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/base/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/base/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/base/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/base/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/base/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/base/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/base/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/base/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/base/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bellcurve/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bellcurve/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bellcurve/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/boxplot/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/boxplot/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bubble/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bubble/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bullet/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/bullet/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bar/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bar/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/base/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/base/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/base/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/boxplot/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/boxplot/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/boxplot/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bullet/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/bullet/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/bullet/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/08.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/08.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/cartesian/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/cartesian/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/connections/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/connections/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/geometric/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/geometric/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/world.geo.json` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.geo.json`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/map_data/map_data/world.topo.json` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/map_data/map_data/world.topo.json`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/pie/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/range/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/range/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-04.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-04.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-05.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-05.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/single_point/error-06.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/single_point/error-06.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/sunburst/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/vector/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/vector/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/venn/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/venn/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/wordcloud/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/data/wordcloud/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/data/wordcloud/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/dependencywheel/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/dependencywheel/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/dependencywheel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/dumbbell/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/dumbbell/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/dumbbell/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/funnel/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/funnel/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/gauge/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/gauge/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/generic/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/generic/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/generic/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/generic/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/heatmap/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/heatmap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/histogram/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/histogram/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/histogram/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/item/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/item/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/item/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/item/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/item/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/item/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/item/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/map/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/map/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mapbubble/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mapbubble/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mapbubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mapline/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mapline/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mapline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mappoint/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/01.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: ASCII text*

 * *Files 1% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 00000000: 7b0a 2020 6461 7461 3a20 5b0a 2020 2020  {.  data: [.    
 00000010: 7b0a 2020 2020 2020 6c61 743a 2035 342e  {.      lat: 54.
 00000020: 3332 312c 0a20 2020 2020 206c 6f6e 3a20  321,.      lon: 
 00000030: 3132 2e33 3435 2c0a 2020 2020 2020 783a  12.345,.      x:
 00000040: 2035 2c0a 2020 2020 2020 793a 2031 302c   5,.      y: 10,
 00000050: 0a20 2020 2020 2064 6174 614c 6162 656c  .      dataLabel
-00000060: 733a 2020 7b0a 2020 2020 2020 2020 616c  s:  {.        al
-00000070: 6967 6e3a 2027 6365 6e74 6572 272c 0a20  ign: 'center',. 
-00000080: 2020 2020 2020 2061 6c6c 6f77 4f76 6572         allowOver
-00000090: 6c61 703a 2074 7275 652c 0a20 2020 2020  lap: true,.     
-000000a0: 2020 2061 6e69 6d61 7469 6f6e 3a20 7b0a     animation: {.
-000000b0: 2020 2020 2020 2020 2020 2020 6465 6665              defe
-000000c0: 723a 2035 0a20 2020 2020 2020 207d 2c0a  r: 5.        },.
-000000d0: 2020 2020 2020 2020 6261 636b 6772 6f75          backgrou
-000000e0: 6e64 436f 6c6f 723a 207b 0a20 2020 2020  ndColor: {.     
-000000f0: 2020 2020 2020 206c 696e 6561 7247 7261         linearGra
-00000100: 6469 656e 743a 207b 0a20 2020 2020 2020  dient: {.       
-00000110: 2020 2020 2020 2020 2078 313a 2030 2e31           x1: 0.1
-00000120: 3233 2c0a 2020 2020 2020 2020 2020 2020  23,.            
-00000130: 2020 2020 7832 3a20 302e 3233 342c 0a20      x2: 0.234,. 
-00000140: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-00000150: 313a 2030 2e33 3435 2c0a 2020 2020 2020  1: 0.345,.      
-00000160: 2020 2020 2020 2020 2020 7932 3a20 302e            y2: 0.
-00000170: 3435 360a 2020 2020 2020 2020 2020 2020  456.            
-00000180: 7d2c 0a20 2020 2020 2020 2020 2020 2073  },.            s
-00000190: 746f 7073 3a20 5b0a 2020 2020 2020 2020  tops: [.        
-000001a0: 2020 2020 2020 2020 5b30 2e31 322c 2027          [0.12, '
-000001b0: 2339 3939 275d 2c0a 2020 2020 2020 2020  #999'],.        
-000001c0: 2020 2020 2020 2020 5b30 2e33 342c 2027          [0.34, '
-000001d0: 2366 6666 275d 0a20 2020 2020 2020 2020  #fff'].         
-000001e0: 2020 205d 0a20 2020 2020 2020 207d 2c0a     ].        },.
-000001f0: 2020 2020 2020 2020 626f 7264 6572 436f          borderCo
-00000200: 6c6f 723a 2027 2339 3939 3939 3927 2c0a  lor: '#999999',.
-00000210: 2020 2020 2020 2020 626f 7264 6572 5261          borderRa
-00000220: 6469 7573 3a20 3234 2c0a 2020 2020 2020  dius: 24,.      
-00000230: 2020 626f 7264 6572 5769 6474 683a 2031    borderWidth: 1
-00000240: 2c0a 2020 2020 2020 2020 636c 6173 734e  ,.        classN
-00000250: 616d 653a 2027 736f 6d65 2d63 6c61 7373  ame: 'some-class
-00000260: 2d6e 616d 6527 2c0a 2020 2020 2020 2020  -name',.        
-00000270: 636f 6c6f 723a 2027 2330 3030 3030 3027  color: '#000000'
-00000280: 2c0a 2020 2020 2020 2020 6372 6f70 3a20  ,.        crop: 
-00000290: 7472 7565 2c0a 2020 2020 2020 2020 6465  true,.        de
-000002a0: 6665 723a 2066 616c 7365 2c0a 2020 2020  fer: false,.    
-000002b0: 2020 2020 656e 6162 6c65 643a 2074 7275      enabled: tru
-000002c0: 652c 0a20 2020 2020 2020 2066 696c 7465  e,.        filte
-000002d0: 723a 207b 0a20 2020 2020 2020 2020 2020  r: {.           
-000002e0: 206f 7065 7261 746f 723a 2027 3e3d 272c   operator: '>=',
-000002f0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000300: 7065 7274 793a 2027 736f 6d65 5f70 726f  perty: 'some_pro
-00000310: 7065 7274 7927 2c0a 2020 2020 2020 2020  perty',.        
-00000320: 2020 2020 7661 6c75 653a 2031 3233 0a20      value: 123. 
-00000330: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00000340: 2020 666f 726d 6174 3a20 2773 6f6d 6520    format: 'some 
-00000350: 666f 726d 6174 272c 0a20 2020 2020 2020  format',.       
-00000360: 2066 6f72 6d61 7474 6572 3a20 6675 6e63   formatter: func
-00000370: 7469 6f6e 2829 207b 2072 6574 7572 6e20  tion() { return 
-00000380: 7472 7565 3b20 7d2c 0a20 2020 2020 2020  true; },.       
-00000390: 2069 6e73 6964 653a 2074 7275 652c 0a20   inside: true,. 
-000003a0: 2020 2020 2020 206e 756c 6c46 6f72 6d61         nullForma
-000003b0: 743a 2027 736f 6d65 2066 6f72 6d61 7427  t: 'some format'
-000003c0: 2c0a 2020 2020 2020 2020 6e75 6c6c 466f  ,.        nullFo
-000003d0: 726d 6174 7465 723a 2066 756e 6374 696f  rmatter: functio
-000003e0: 6e28 2920 7b20 7265 7475 726e 2074 7275  n() { return tru
-000003f0: 653b 207d 2c0a 2020 2020 2020 2020 6f76  e; },.        ov
-00000400: 6572 666c 6f77 3a20 276e 6f6e 6527 2c0a  erflow: 'none',.
-00000410: 2020 2020 2020 2020 7061 6464 696e 673a          padding:
-00000420: 2031 322c 0a20 2020 2020 2020 2070 6f73   12,.        pos
-00000430: 6974 696f 6e3a 2027 6365 6e74 6572 272c  ition: 'center',
-00000440: 0a20 2020 2020 2020 2072 6f74 6174 696f  .        rotatio
-00000450: 6e3a 2030 2c0a 2020 2020 2020 2020 7368  n: 0,.        sh
-00000460: 6164 6f77 3a20 6661 6c73 652c 0a20 2020  adow: false,.   
-00000470: 2020 2020 2073 6861 7065 3a20 2772 6563       shape: 'rec
-00000480: 7427 2c0a 2020 2020 2020 2020 7374 796c  t',.        styl
-00000490: 653a 2027 7374 796c 6520 676f 6573 2068  e: 'style goes h
-000004a0: 6572 6527 2c0a 2020 2020 2020 2020 7573  ere',.        us
-000004b0: 6548 544d 4c3a 2066 616c 7365 2c0a 2020  eHTML: false,.  
-000004c0: 2020 2020 2020 7665 7274 6963 616c 416c        verticalAl
-000004d0: 6967 6e3a 2027 746f 7027 2c0a 2020 2020  ign: 'top',.    
-000004e0: 2020 2020 783a 2031 302c 0a20 2020 2020      x: 10,.     
-000004f0: 2020 2079 3a20 3230 2c0a 2020 2020 2020     y: 20,.      
-00000500: 2020 7a3a 2030 0a20 2020 2020 207d 2c0a    z: 0.      },.
-00000510: 2020 2020 2020 6472 696c 6c64 6f77 6e3a        drilldown:
-00000520: 2027 736f 6d65 2d69 642d 676f 6573 2d68   'some-id-goes-h
-00000530: 6572 6527 2c0a 2020 2020 2020 6765 6f6d  ere',.      geom
-00000540: 6574 7279 3a20 7b0a 2020 2020 2020 2020  etry: {.        
-00000550: 2267 656f 6d65 7472 7922 3a20 7b0a 2020  "geometry": {.  
-00000560: 2020 2020 2020 2020 2263 6f6f 7264 696e          "coordin
-00000570: 6174 6573 223a 205b 0a20 2020 2020 2020  ates": [.       
-00000580: 2020 2020 202d 332e 3638 2c0a 2020 2020       -3.68,.    
-00000590: 2020 2020 2020 2020 3430 2e34 0a20 2020          40.4.   
-000005a0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-000005b0: 2020 2020 2274 7970 6522 3a20 2250 6f69      "type": "Poi
-000005c0: 6e74 220a 2020 2020 2020 2020 7d2c 0a20  nt".        },. 
-000005d0: 2020 2020 2020 2022 7072 6f70 6572 7469         "properti
-000005e0: 6573 223a 207b 7d2c 0a20 2020 2020 2020  es": {},.       
-000005f0: 2022 7479 7065 223a 2022 4665 6174 7572   "type": "Featur
-00000600: 6522 0a20 2020 2020 207d 0a20 2020 207d  e".      }.    }
-00000610: 0a20 205d 2c0a 0a20 206e 6567 6174 6976  .  ],..  negativ
-00000620: 6543 6f6c 6f72 3a20 2723 3030 3027 2c0a  eColor: '#000',.
-00000630: 2020 616e 696d 6174 696f 6e4c 696d 6974    animationLimit
-00000640: 3a20 3235 302c 0a20 200a 2020 6461 7461  : 250,.  .  data
-00000650: 4173 436f 6c75 6d6e 733a 2066 616c 7365  AsColumns: false
-00000660: 2c0a 0a20 2061 6c6c 4172 6561 733a 2074  ,..  allAreas: t
-00000670: 7275 652c 0a20 206a 6f69 6e42 793a 2027  rue,.  joinBy: '
-00000680: 6863 2d6b 6579 270a 7d0a                 hc-key'.}.
+00000060: 733a 207b 0a20 2020 2020 2020 2061 6c69  s: {.        ali
+00000070: 676e 3a20 2763 656e 7465 7227 2c0a 2020  gn: 'center',.  
+00000080: 2020 2020 2020 616c 6c6f 774f 7665 726c        allowOverl
+00000090: 6170 3a20 7472 7565 2c0a 2020 2020 2020  ap: true,.      
+000000a0: 2020 616e 696d 6174 696f 6e3a 207b 0a20    animation: {. 
+000000b0: 2020 2020 2020 2020 2020 2064 6566 6572             defer
+000000c0: 3a20 350a 2020 2020 2020 2020 7d2c 0a20  : 5.        },. 
+000000d0: 2020 2020 2020 2062 6163 6b67 726f 756e         backgroun
+000000e0: 6443 6f6c 6f72 3a20 7b0a 2020 2020 2020  dColor: {.      
+000000f0: 2020 2020 2020 6c69 6e65 6172 4772 6164        linearGrad
+00000100: 6965 6e74 3a20 7b0a 2020 2020 2020 2020  ient: {.        
+00000110: 2020 2020 2020 2020 7831 3a20 302e 3132          x1: 0.12
+00000120: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+00000130: 2020 2078 323a 2030 2e32 3334 2c0a 2020     x2: 0.234,.  
+00000140: 2020 2020 2020 2020 2020 2020 2020 7931                y1
+00000150: 3a20 302e 3334 352c 0a20 2020 2020 2020  : 0.345,.       
+00000160: 2020 2020 2020 2020 2079 323a 2030 2e34           y2: 0.4
+00000170: 3536 0a20 2020 2020 2020 2020 2020 207d  56.            }
+00000180: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+00000190: 6f70 733a 205b 0a20 2020 2020 2020 2020  ops: [.         
+000001a0: 2020 2020 2020 205b 302e 3132 2c20 2723         [0.12, '#
+000001b0: 3939 3927 5d2c 0a20 2020 2020 2020 2020  999'],.         
+000001c0: 2020 2020 2020 205b 302e 3334 2c20 2723         [0.34, '#
+000001d0: 6666 6627 5d0a 2020 2020 2020 2020 2020  fff'].          
+000001e0: 2020 5d0a 2020 2020 2020 2020 7d2c 0a20    ].        },. 
+000001f0: 2020 2020 2020 2062 6f72 6465 7243 6f6c         borderCol
+00000200: 6f72 3a20 2723 3939 3939 3939 272c 0a20  or: '#999999',. 
+00000210: 2020 2020 2020 2062 6f72 6465 7252 6164         borderRad
+00000220: 6975 733a 2032 342c 0a20 2020 2020 2020  ius: 24,.       
+00000230: 2062 6f72 6465 7257 6964 7468 3a20 312c   borderWidth: 1,
+00000240: 0a20 2020 2020 2020 2063 6c61 7373 4e61  .        classNa
+00000250: 6d65 3a20 2773 6f6d 652d 636c 6173 732d  me: 'some-class-
+00000260: 6e61 6d65 272c 0a20 2020 2020 2020 2063  name',.        c
+00000270: 6f6c 6f72 3a20 2723 3030 3030 3030 272c  olor: '#000000',
+00000280: 0a20 2020 2020 2020 2063 726f 703a 2074  .        crop: t
+00000290: 7275 652c 0a20 2020 2020 2020 2064 6566  rue,.        def
+000002a0: 6572 3a20 6661 6c73 652c 0a20 2020 2020  er: false,.     
+000002b0: 2020 2065 6e61 626c 6564 3a20 7472 7565     enabled: true
+000002c0: 2c0a 2020 2020 2020 2020 6669 6c74 6572  ,.        filter
+000002d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+000002e0: 6f70 6572 6174 6f72 3a20 273e 3d27 2c0a  operator: '>=',.
+000002f0: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
+00000300: 6572 7479 3a20 2773 6f6d 655f 7072 6f70  erty: 'some_prop
+00000310: 6572 7479 272c 0a20 2020 2020 2020 2020  erty',.         
+00000320: 2020 2076 616c 7565 3a20 3132 330a 2020     value: 123.  
+00000330: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000340: 2066 6f72 6d61 743a 2027 736f 6d65 2066   format: 'some f
+00000350: 6f72 6d61 7427 2c0a 2020 2020 2020 2020  ormat',.        
+00000360: 666f 726d 6174 7465 723a 2066 756e 6374  formatter: funct
+00000370: 696f 6e28 2920 7b20 7265 7475 726e 2074  ion() { return t
+00000380: 7275 653b 207d 2c0a 2020 2020 2020 2020  rue; },.        
+00000390: 696e 7369 6465 3a20 7472 7565 2c0a 2020  inside: true,.  
+000003a0: 2020 2020 2020 6e75 6c6c 466f 726d 6174        nullFormat
+000003b0: 3a20 2773 6f6d 6520 666f 726d 6174 272c  : 'some format',
+000003c0: 0a20 2020 2020 2020 206e 756c 6c46 6f72  .        nullFor
+000003d0: 6d61 7474 6572 3a20 6675 6e63 7469 6f6e  matter: function
+000003e0: 2829 207b 2072 6574 7572 6e20 7472 7565  () { return true
+000003f0: 3b20 7d2c 0a20 2020 2020 2020 206f 7665  ; },.        ove
+00000400: 7266 6c6f 773a 2027 6e6f 6e65 272c 0a20  rflow: 'none',. 
+00000410: 2020 2020 2020 2070 6164 6469 6e67 3a20         padding: 
+00000420: 3132 2c0a 2020 2020 2020 2020 706f 7369  12,.        posi
+00000430: 7469 6f6e 3a20 2763 656e 7465 7227 2c0a  tion: 'center',.
+00000440: 2020 2020 2020 2020 726f 7461 7469 6f6e          rotation
+00000450: 3a20 302c 0a20 2020 2020 2020 2073 6861  : 0,.        sha
+00000460: 646f 773a 2066 616c 7365 2c0a 2020 2020  dow: false,.    
+00000470: 2020 2020 7368 6170 653a 2027 7265 6374      shape: 'rect
+00000480: 272c 0a20 2020 2020 2020 2073 7479 6c65  ',.        style
+00000490: 3a20 2773 7479 6c65 2067 6f65 7320 6865  : 'style goes he
+000004a0: 7265 272c 0a20 2020 2020 2020 2075 7365  re',.        use
+000004b0: 4854 4d4c 3a20 6661 6c73 652c 0a20 2020  HTML: false,.   
+000004c0: 2020 2020 2076 6572 7469 6361 6c41 6c69       verticalAli
+000004d0: 676e 3a20 2774 6f70 272c 0a20 2020 2020  gn: 'top',.     
+000004e0: 2020 2078 3a20 3130 2c0a 2020 2020 2020     x: 10,.      
+000004f0: 2020 793a 2032 302c 0a20 2020 2020 2020    y: 20,.       
+00000500: 207a 3a20 300a 2020 2020 2020 7d2c 0a20   z: 0.      },. 
+00000510: 2020 2020 2064 7269 6c6c 646f 776e 3a20       drilldown: 
+00000520: 2773 6f6d 652d 6964 2d67 6f65 732d 6865  'some-id-goes-he
+00000530: 7265 272c 0a20 2020 2020 2067 656f 6d65  re',.      geome
+00000540: 7472 793a 207b 0a20 2020 2020 2020 2022  try: {.        "
+00000550: 6765 6f6d 6574 7279 223a 207b 0a20 2020  geometry": {.   
+00000560: 2020 2020 2020 2022 636f 6f72 6469 6e61         "coordina
+00000570: 7465 7322 3a20 5b0a 2020 2020 2020 2020  tes": [.        
+00000580: 2020 2020 2d33 2e36 382c 0a20 2020 2020      -3.68,.     
+00000590: 2020 2020 2020 2034 302e 340a 2020 2020         40.4.    
+000005a0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+000005b0: 2020 2022 7479 7065 223a 2022 506f 696e     "type": "Poin
+000005c0: 7422 0a20 2020 2020 2020 207d 2c0a 2020  t".        },.  
+000005d0: 2020 2020 2020 2270 726f 7065 7274 6965        "propertie
+000005e0: 7322 3a20 7b7d 2c0a 2020 2020 2020 2020  s": {},.        
+000005f0: 2274 7970 6522 3a20 2246 6561 7475 7265  "type": "Feature
+00000600: 220a 2020 2020 2020 7d0a 2020 2020 7d0a  ".      }.    }.
+00000610: 2020 5d2c 0a0a 2020 6e65 6761 7469 7665    ],..  negative
+00000620: 436f 6c6f 723a 2027 2330 3030 272c 0a20  Color: '#000',. 
+00000630: 2061 6e69 6d61 7469 6f6e 4c69 6d69 743a   animationLimit:
+00000640: 2032 3530 2c0a 2020 0a20 2064 6174 6141   250,.  .  dataA
+00000650: 7343 6f6c 756d 6e73 3a20 6661 6c73 652c  sColumns: false,
+00000660: 0a0a 2020 616c 6c41 7265 6173 3a20 7472  ..  allAreas: tr
+00000670: 7565 2c0a 2020 6a6f 696e 4279 3a20 2768  ue,.  joinBy: 'h
+00000680: 632d 6b65 7927 0a7d 0a                   c-key'.}.
```

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/mappoint/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/mappoint/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/networkgraph/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/networkgraph/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/organization/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/organization/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/organization/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/organization/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/organization/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/packedbubble/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/packedbubble/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pareto/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pareto/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pie/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pie/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pie/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/pie/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/pie/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/polygon/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/polygon/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sankey/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sankey/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/scatter/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/scatter/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/spline/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/spline/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/spline/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/spline/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/spline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/sunburst/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/sunburst/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/timeline/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/timeline/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/treemap/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/treemap/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/vector/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/vector/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/vector/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/vector/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/vector/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/venn/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/venn/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/venn/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/venn/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/venn/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/series/wordcloud/error-02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/series/wordcloud/error-02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/test-data-files/nst-est2019-01-transposed.csv` & `highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01-transposed.csv`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/test-data-files/nst-est2019-01.csv` & `highcharts_maps-1.0.0rc6/tests/input_files/test-data-files/nst-est2019-01.csv`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/clusters/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/clusters/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/clusters/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_grouping/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_grouping/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_grouping/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/02.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/02.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/error-01.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-01.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/input_files/utility_classes/data_labels/error-03.js` & `highcharts_maps-1.0.0rc6/tests/input_files/utility_classes/data_labels/error-03.js`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_boost.py` & `highcharts_maps-1.0.0rc6/tests/options/test_boost.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_caption.py` & `highcharts_maps-1.0.0rc6/tests/options/test_caption.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_credits.py` & `highcharts_maps-1.0.0rc6/tests/options/test_credits.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_data.py` & `highcharts_maps-1.0.0rc6/tests/options/test_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_defs.py` & `highcharts_maps-1.0.0rc6/tests/options/test_defs.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_drilldown.py` & `highcharts_maps-1.0.0rc6/tests/options/test_drilldown.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_loading.py` & `highcharts_maps-1.0.0rc6/tests/options/test_loading.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_options.py` & `highcharts_maps-1.0.0rc6/tests/options/test_options.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_responsive.py` & `highcharts_maps-1.0.0rc6/tests/options/test_responsive.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_subtitle.py` & `highcharts_maps-1.0.0rc6/tests/options/test_subtitle.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_time.py` & `highcharts_maps-1.0.0rc6/tests/options/test_time.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_title.py` & `highcharts_maps-1.0.0rc6/tests/options/test_title.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/test_tooltips.py` & `highcharts_maps-1.0.0rc6/tests/options/test_tooltips.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/accessibility/test_accessibility.py` & `highcharts_maps-1.0.0rc6/tests/options/accessibility/test_accessibility.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/annotations/test_annotation.py` & `highcharts_maps-1.0.0rc6/tests/options/annotations/test_annotation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_color_axis.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_color_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_numeric.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_numeric.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_parallel_axes.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_parallel_axes.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_plot_bands.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_plot_bands.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_x_axis.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_x_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_y_axis.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_y_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/axes/test_z_axis.py` & `highcharts_maps-1.0.0rc6/tests/options/axes/test_z_axis.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/chart/test_chart.py` & `highcharts_maps-1.0.0rc6/tests/options/chart/test_chart.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/chart/test_options_3d.py` & `highcharts_maps-1.0.0rc6/tests/options/chart/test_options_3d.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/chart/test_zooming.py` & `highcharts_maps-1.0.0rc6/tests/options/chart/test_zooming.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/exporting/test_csv.py` & `highcharts_maps-1.0.0rc6/tests/options/exporting/test_csv.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/exporting/test_exporting.py` & `highcharts_maps-1.0.0rc6/tests/options/exporting/test_exporting.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/legend/test_bubble_legend.py` & `highcharts_maps-1.0.0rc6/tests/options/legend/test_bubble_legend.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/legend/test_legend.py` & `highcharts_maps-1.0.0rc6/tests/options/legend/test_legend.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/legend/test_navigation.py` & `highcharts_maps-1.0.0rc6/tests/options/legend/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/navigation/test_bindings.py` & `highcharts_maps-1.0.0rc6/tests/options/navigation/test_bindings.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/navigation/test_navigation.py` & `highcharts_maps-1.0.0rc6/tests/options/navigation/test_navigation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_PlotOptions.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_PlotOptions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_arcdiagram.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_arcdiagram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_area.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_area.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bar.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bellcurve.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bellcurve.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_boxplot.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bubble.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_bullet.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_dependencywheel.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dependencywheel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_dumbbell.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_dumbbell.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_funnel.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_funnel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_gauge.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_gauge.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_generic.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_generic.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_heatmap.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_histogram.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_histogram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_item.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_item.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_map.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mapbubble.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mapline.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_mappoint.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_networkgraph.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_networkgraph.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_organization.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_organization.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_packedbubble.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_packedbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pareto.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pareto.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pie.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_polygon.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_polygon.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_pyramid.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_sankey.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sankey.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_scatter.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_scatter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_series.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_series.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_spline.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_spline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_sunburst.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_timeline.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_timeline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_treemap.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_treemap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_vector.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_venn.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/plot_options/test_wordcloud.py` & `highcharts_maps-1.0.0rc6/tests/options/plot_options/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_arcdiagram.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_arcdiagram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_area.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_area.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_bar.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_base.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_bellcurve.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_bellcurve.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_boxplot.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_bubble.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_bubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_bullet.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_dependencywheel.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_dependencywheel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_dumbbell.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_dumbbell.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_funnel.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_funnel.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_gauge.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_gauge.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_heatmap.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_histogram.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_histogram.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_item.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_item.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_map.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_map.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_mapbubble.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_mapbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_mapline.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_mapline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_mappoint.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_mappoint.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_networkgraph.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_networkgraph.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_organization.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_organization.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_packedbubble.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_packedbubble.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_pareto.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_pareto.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_pie.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_polygon.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_polygon.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_pyramid.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_sankey.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_sankey.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_scatter.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_scatter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_spline.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_spline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_sunburst.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_timeline.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_timeline.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_treemap.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_treemap.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_vector.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_venn.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/test_wordcloud.py` & `highcharts_maps-1.0.0rc6/tests/options/series/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_bar.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_bar.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_base.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_base.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_boxplot.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_boxplot.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_bullet.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_bullet.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_cartesian.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_connections.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_connections.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_geometric.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_geometric.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_map_data.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_map_data.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_pie.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_pie.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_range.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_range.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_single_point.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_single_point.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_sunburst.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_vector.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_vector.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_venn.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_venn.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/options/series/data/test_wordcloud.py` & `highcharts_maps-1.0.0rc6/tests/options/series/data/test_wordcloud.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_animation.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_animation.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_ast.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_ast.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_breadcrumbs.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_buttons.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_buttons.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_clusters.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_clusters.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_data_grouping.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_grouping.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_data_labels.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_data_labels.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_date_time_label_formats.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_date_time_label_formats.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_events.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_events.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_gradients.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_gradients.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_javascript_functions.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_javascript_functions.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_jitter.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_jitter.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_markers.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_markers.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_menus.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_menus.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_nodes.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_nodes.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_partial_fill.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_partial_fill.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_patterns.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_patterns.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_position.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_position.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_shadows.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_shadows.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_states.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_states.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/tests/utility_classes/test_zones.py` & `highcharts_maps-1.0.0rc6/tests/utility_classes/test_zones.py`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/.gitignore` & `highcharts_maps-1.0.0rc6/.gitignore`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/LICENSE` & `highcharts_maps-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/README.rst` & `highcharts_maps-1.0.0rc6/README.rst`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/pyproject.toml` & `highcharts_maps-1.0.0rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `highcharts_maps-1.0.0rc5/PKG-INFO` & `highcharts_maps-1.0.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: highcharts-maps
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: High-end Map Data Visualization for the Python Ecosystem
 Project-URL: Homepage, https://www.highchartspython.com
 Project-URL: Documentation, https://maps-docs.highchartspython.com/en/latest/
 Project-URL: Support, https://www.highchartspython.com/get-help
 Project-URL: Source Code, https://github.com/highcharts-for-python/highcharts-maps
 Project-URL: History, https://github.com/highcharts-for-python/highcharts-maps/blob/master/CHANGES.rst
 Project-URL: Bug Tracker, https://github.com/highcharts-for-python/highcharts-maps/issues
```

