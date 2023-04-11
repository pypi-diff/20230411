# Comparing `tmp/openbb_nightly-3.0.0rc1.dev20230410.tar.gz` & `tmp/openbb_nightly-3.0.0rc1.dev20230411.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-3.0.0rc1.dev20230410.tar", max compression
+gzip compressed data, was "openbb_nightly-3.0.0rc1.dev20230411.tar", max compression
```

## Comparing `openbb_nightly-3.0.0rc1.dev20230410.tar` & `openbb_nightly-3.0.0rc1.dev20230411.tar`

### file list

```diff
@@ -1,964 +1,964 @@
--rw-r--r--   0        0        0     1073 2023-04-10 00:09:07.237163 openbb_nightly-3.0.0rc1.dev20230410/LICENSE
--rw-r--r--   0        0        0    18588 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/SDK_README.md
--rw-r--r--   0        0        0      243 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/__init__.py
--rw-r--r--   0        0        0    19834 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_controller.py
--rw-r--r--   0        0        0     3382 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_model.py
--rw-r--r--   0        0        0      612 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/__init__.py
--rw-r--r--   0        0        0     3131 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/alt_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/__init__.py
--rw-r--r--   0        0        0     1881 2023-04-10 00:09:07.409164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/countries.txt
--rw-r--r--   0        0        0     9347 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_controller.py
--rw-r--r--   0        0        0     5387 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_model.py
--rw-r--r--   0        0        0     8586 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_view.py
--rw-r--r--   0        0        0     1070 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/hackernews_model.py
--rw-r--r--   0        0        0     1087 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/hackernews_view.py
--rw-r--r--   0        0        0     6752 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/github_model.py
--rw-r--r--   0        0        0     3968 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/github_view.py
--rw-r--r--   0        0        0     8656 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/oss_controller.py
--rw-r--r--   0        0        0     4437 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/runa_model.py
--rw-r--r--   0        0        0     4018 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/runa_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/__init__.py
--rw-r--r--   0        0        0     9030 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/landRegistry_model.py
--rw-r--r--   0        0        0     3309 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/landRegistry_view.py
--rw-r--r--   0        0        0     8108 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/realestate_controller.py
--rw-r--r--   0        0        0     2718 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/base_helpers.py
--rw-r--r--   0        0        0       93 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0     1198 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finbrain_model.py
--rw-r--r--   0        0        0     4394 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1335 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     1861 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3329 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/google_model.py
--rw-r--r--   0        0        0     7118 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/google_view.py
--rw-r--r--   0        0        0     5524 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
--rw-r--r--   0        0        0    18297 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_model.py
--rw-r--r--   0        0        0    10206 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_view.py
--rw-r--r--   0        0        0     3239 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
--rw-r--r--   0        0        0     2898 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
--rw-r--r--   0        0        0     6160 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/twitter_model.py
--rw-r--r--   0        0        0     5870 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/twitter_view.py
--rw-r--r--   0        0        0     4142 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/common_model.py
--rw-r--r--   0        0        0     3634 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/feedparser_model.py
--rw-r--r--   0        0        0     1242 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/feedparser_view.py
--rw-r--r--   0        0        0     2639 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/newsapi_model.py
--rw-r--r--   0        0        0     1465 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/newsapi_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    19923 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0    32308 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/qa_view.py
--rw-r--r--   0        0        0     3226 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/rolling_model.py
--rw-r--r--   0        0        0    10790 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/rolling_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/__init__.py
--rw-r--r--   0        0        0     2977 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/custom_indicators_model.py
--rw-r--r--   0        0        0     4272 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/custom_indicators_view.py
--rw-r--r--   0        0        0     6427 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/momentum_model.py
--rw-r--r--   0        0        0    10556 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/momentum_view.py
--rw-r--r--   0        0        0     4179 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/overlap_model.py
--rw-r--r--   0        0        0     4361 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/overlap_view.py
--rw-r--r--   0        0        0     1453 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/ta_helpers.py
--rw-r--r--   0        0        0     1819 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/trend_indicators_model.py
--rw-r--r--   0        0        0     2621 2023-04-10 00:09:07.413164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/trend_indicators_view.py
--rw-r--r--   0        0        0    19962 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volatility_model.py
--rw-r--r--   0        0        0    10008 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volatility_view.py
--rw-r--r--   0        0        0     2614 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volume_model.py
--rw-r--r--   0        0        0     3806 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volume_view.py
--rw-r--r--   0        0        0     5813 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/ultima_newsmonitor_model.py
--rw-r--r--   0        0        0     3886 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/ultima_newsmonitor_view.py
--rw-r--r--   0        0        0     2634 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/config_terminal.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/__init__.py
--rw-r--r--   0        0        0     9829 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/completer/choices.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/config/__init__.py
--rw-r--r--   0        0        0      927 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/config/paths.py
--rw-r--r--   0        0        0     2650 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/config/paths_helper.py
--rw-r--r--   0        0        0     9162 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/integration_tests/README.md
--rw-r--r--   0        0        0    21758 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/integration_tests/integration_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/__init__.py
--rw-r--r--   0        0        0     3848 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/log_sender.py
--rw-r--r--   0        0        0     3744 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/logging_clock.py
--rw-r--r--   0        0        0     3495 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/s3_sender.py
--rw-r--r--   0        0        0      166 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/constants.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/__init__.py
--rw-r--r--   0        0        0      524 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/common.py
--rw-r--r--   0        0        0      525 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/custom_logger.py
--rw-r--r--   0        0        0      979 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/directories.py
--rw-r--r--   0        0        0      841 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/expired_files.py
--rw-r--r--   0        0        0     4896 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/formatter_with_exceptions.py
--rw-r--r--   0        0        0     6058 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4166 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/settings.py
--rw-r--r--   0        0        0     1621 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/settings_logger.py
--rw-r--r--   0        0        0      396 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/user_logger.py
--rw-r--r--   0        0        0      627 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/__init__.py
--rw-r--r--   0        0        0     1221 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/base_model.py
--rw-r--r--   0        0        0      818 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/credentials_model.py
--rw-r--r--   0        0        0     4154 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/preferences_model.py
--rw-r--r--   0        0        0     1817 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/profile_model.py
--rw-r--r--   0        0        0     1230 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/sources_model.py
--rw-r--r--   0        0        0     1753 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/system_model.py
--rw-r--r--   0        0        0      562 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/user_model.py
--rw-r--r--   0        0        0      200 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/__init__.py
--rw-r--r--   0        0        0   418780 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/assets/Terminal_icon.png
--rw-r--r--   0        0        0      727 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/assets/icon.png
--rw-r--r--   0        0        0    14854 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/backend.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/config/__init__.py
--rw-r--r--   0        0        0     7156 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/config/openbb_styles.py
--rw-r--r--   0        0        0     3073 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/no_import.py
--rw-r--r--   0        0        0     1261 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/old_table.html
--rw-r--r--   0        0        0     7732 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly.html
--rw-r--r--   0        0        0    62668 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_helper.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.417163 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/__init__.py
--rw-r--r--   0        0        0     6724 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/base.py
--rw-r--r--   0        0        0    11358 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8016 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    15173 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3361 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5683 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6868 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3429 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    20644 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/ta_class.py
--rw-r--r--   0        0        0   704570 2023-04-10 00:09:07.421164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/table.html
--rw-r--r--   0        0        0    11182 2023-04-10 00:09:07.425164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/bar_menus.js
--rw-r--r--   0        0        0   289624 2023-04-10 00:09:07.425164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
--rw-r--r--   0        0        0   286320 2023-04-10 00:09:07.425164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
--rw-r--r--   0        0        0    25188 2023-04-10 00:09:07.425164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/style.css
--rw-r--r--   0        0        0      151 2023-04-10 00:09:07.425164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/table.css
--rw-r--r--   0        0        0    16611 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/helpers.js
--rw-r--r--   0        0        0    12724 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/main.js
--rw-r--r--   0        0        0     3255 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/main_table.js
--rw-r--r--   0        0        0    24525 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/popups.js
--rw-r--r--   0        0        0     7747 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/scripts/sdk_audit.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/__init__.py
--rw-r--r--   0        0        0      450 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/__init__.py
--rw-r--r--   0        0        0     2660 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
--rw-r--r--   0        0        0    24088 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
--rw-r--r--   0        0        0     1513 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
--rw-r--r--   0        0        0     2365 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
--rw-r--r--   0        0        0     5128 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
--rw-r--r--   0        0        0    18447 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
--rw-r--r--   0        0        0      761 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/__init__.py
--rw-r--r--   0        0        0     4308 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/alt_sdk_model.py
--rw-r--r--   0        0        0    42910 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/crypto_sdk_model.py
--rw-r--r--   0        0        0     4497 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
--rw-r--r--   0        0        0     7975 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/economy_sdk_model.py
--rw-r--r--   0        0        0     2496 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/etf_sdk_model.py
--rw-r--r--   0        0        0     3515 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
--rw-r--r--   0        0        0     8550 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/forecast_sdk_model.py
--rw-r--r--   0        0        0     4386 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/forex_sdk_model.py
--rw-r--r--   0        0        0     1530 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/funds_sdk_model.py
--rw-r--r--   0        0        0     1067 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/futures_sdk_model.py
--rw-r--r--   0        0        0     3638 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/keys_sdk_model.py
--rw-r--r--   0        0        0    10046 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
--rw-r--r--   0        0        0     4603 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/qa_sdk_model.py
--rw-r--r--   0        0        0    32674 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/stocks_sdk_model.py
--rw-r--r--   0        0        0     7229 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/ta_sdk_model.py
--rw-r--r--   0        0        0    11508 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/sdk_helpers.py
--rw-r--r--   0        0        0    19813 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/sdk_init.py
--rw-r--r--   0        0        0    43994 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map.csv
--rw-r--r--   0        0        0     2801 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map_forecasting.csv
--rw-r--r--   0        0        0     1301 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map_optimization.csv
--rw-r--r--   0        0        0     7118 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trailmap.py
--rw-r--r--   0        0        0     1017 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/banner.txt
--rw-r--r--   0        0        0      485 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/constants.py
--rw-r--r--   0        0        0     1000 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/current_system.py
--rw-r--r--   0        0        0     4095 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/current_user.py
--rw-r--r--   0        0        0     1147 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/env_handler.py
--rw-r--r--   0        0        0    20665 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/hub_model.py
--rw-r--r--   0        0        0     5477 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/local_model.py
--rw-r--r--   0        0        0     3097 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/sdk_session.py
--rw-r--r--   0        0        0     2913 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/session_controller.py
--rw-r--r--   0        0        0     4656 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/session_model.py
--rw-r--r--   0        0        0     2834 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/sources_handler.py
--rw-r--r--   0        0        0     1551 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/utils.py
--rw-r--r--   0        0        0     3011 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sources/utils.py
--rw-r--r--   0        0        0      199 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/README.md
--rw-r--r--   0        0        0       84 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/__init__.py
--rw-r--r--   0        0        0     5303 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/coinbase_helpers.py
--rw-r--r--   0        0        0     2147 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
--rw-r--r--   0        0        0    19275 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_controller.py
--rw-r--r--   0        0        0     4481 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_models.py
--rw-r--r--   0        0        0     1785 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_views.py
--rw-r--r--   0        0        0    30339 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
--rw-r--r--   0        0        0      949 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/README.md
--rw-r--r--   0        0        0     7341 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
--rw-r--r--   0        0        0     2436 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
--rw-r--r--   0        0        0     4813 2023-04-10 00:09:07.429164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coingecko_categories.json
--rw-r--r--   0        0        0   954385 2023-04-10 00:09:07.433164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coingecko_coins.json
--rw-r--r--   0        0        0  2245016 2023-04-10 00:09:07.441164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
--rw-r--r--   0        0        0    31307 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/defillama_dapps.json
--rw-r--r--   0        0        0   107203 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/erc20_coins.json
--rw-r--r--   0        0        0     7255 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/finbrain_coins.json
--rw-r--r--   0        0        0   222978 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/santiment_slugs.json
--rw-r--r--   0        0        0   300253 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
--rw-r--r--   0        0        0     4951 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/dataframe_helpers.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/__init__.py
--rw-r--r--   0        0        0     4537 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/coindix_model.py
--rw-r--r--   0        0        0     2720 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/coindix_view.py
--rw-r--r--   0        0        0     2483 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
--rw-r--r--   0        0        0     1994 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
--rw-r--r--   0        0        0    31284 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/defi_controller.py
--rw-r--r--   0        0        0     8918 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/graph_model.py
--rw-r--r--   0        0        0     7165 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/graph_view.py
--rw-r--r--   0        0        0     5005 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/llama_model.py
--rw-r--r--   0        0        0     5827 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/llama_view.py
--rw-r--r--   0        0        0     1808 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/smartstake_model.py
--rw-r--r--   0        0        0     3110 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/smartstake_view.py
--rw-r--r--   0        0        0     2882 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/substack_model.py
--rw-r--r--   0        0        0     1090 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/substack_view.py
--rw-r--r--   0        0        0     1947 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
--rw-r--r--   0        0        0     2699 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
--rw-r--r--   0        0        0     9734 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
--rw-r--r--   0        0        0     8022 2023-04-10 00:09:07.445164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/__init__.py
--rw-r--r--   0        0        0     2317 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
--rw-r--r--   0        0        0     1620 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
--rw-r--r--   0        0        0     2116 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
--rw-r--r--   0        0        0     1936 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
--rw-r--r--   0        0        0     7614 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
--rw-r--r--   0        0        0     5045 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
--rw-r--r--   0        0        0    21019 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
--rw-r--r--   0        0        0    10833 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
--rw-r--r--   0        0        0     6352 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
--rw-r--r--   0        0        0     1095 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/__init__.py
--rw-r--r--   0        0        0     7483 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
--rw-r--r--   0        0        0     3009 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
--rw-r--r--   0        0        0     3188 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
--rw-r--r--   0        0        0     2840 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
--rw-r--r--   0        0        0     6439 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
--rw-r--r--   0        0        0     4134 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
--rw-r--r--   0        0        0     6587 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
--rw-r--r--   0        0        0     6638 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
--rw-r--r--   0        0        0    15062 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
--rw-r--r--   0        0        0     9133 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
--rw-r--r--   0        0        0     2332 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
--rw-r--r--   0        0        0    64101 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
--rw-r--r--   0        0        0     1850 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
--rw-r--r--   0        0        0    15044 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
--rw-r--r--   0        0        0    11237 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
--rw-r--r--   0        0        0    24480 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
--rw-r--r--   0        0        0    22260 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
--rw-r--r--   0        0        0    25887 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
--rw-r--r--   0        0        0     8762 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
--rw-r--r--   0        0        0     3076 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
--rw-r--r--   0        0        0     2070 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
--rw-r--r--   0        0        0     2508 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
--rw-r--r--   0        0        0     6001 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
--rw-r--r--   0        0        0     3474 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/__init__.py
--rw-r--r--   0        0        0     5562 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nft_controller.py
--rw-r--r--   0        0        0     1664 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
--rw-r--r--   0        0        0     4495 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
--rw-r--r--   0        0        0     2895 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/opensea_model.py
--rw-r--r--   0        0        0     1289 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/opensea_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/__init__.py
--rw-r--r--   0        0        0    21848 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
--rw-r--r--   0        0        0    11444 2023-04-10 00:09:07.449164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
--rw-r--r--   0        0        0     3393 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
--rw-r--r--   0        0        0     4733 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
--rw-r--r--   0        0        0     1840 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
--rw-r--r--   0        0        0     1266 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
--rw-r--r--   0        0        0    15974 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
--rw-r--r--   0        0        0    10572 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
--rw-r--r--   0        0        0    53494 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
--rw-r--r--   0        0        0     5938 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/shroom_model.py
--rw-r--r--   0        0        0     5144 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/shroom_view.py
--rw-r--r--   0        0        0     4772 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
--rw-r--r--   0        0        0     2088 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/__init__.py
--rw-r--r--   0        0        0     2274 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
--rw-r--r--   0        0        0     2664 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
--rw-r--r--   0        0        0     1464 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinbase_model.py
--rw-r--r--   0        0        0     1342 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinbase_view.py
--rw-r--r--   0        0        0    11841 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
--rw-r--r--   0        0        0     9646 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
--rw-r--r--   0        0        0     6776 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
--rw-r--r--   0        0        0     2278 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
--rw-r--r--   0        0        0     1100 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/glassnode_model.py
--rw-r--r--   0        0        0     4677 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/glassnode_view.py
--rw-r--r--   0        0        0     5936 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/loanscan_model.py
--rw-r--r--   0        0        0     3279 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/loanscan_view.py
--rw-r--r--   0        0        0    55381 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/overview_controller.py
--rw-r--r--   0        0        0    13641 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
--rw-r--r--   0        0        0    21320 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
--rw-r--r--   0        0        0     5346 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/rekt_model.py
--rw-r--r--   0        0        0     2253 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/rekt_view.py
--rw-r--r--   0        0        0     2042 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
--rw-r--r--   0        0        0     7167 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
--rw-r--r--   0        0        0     3126 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
--rw-r--r--   0        0        0     6708 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
--rw-r--r--   0        0        0     3480 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
--rw-r--r--   0        0        0     7635 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
--rw-r--r--   0        0        0     5693 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pyth_model.py
--rw-r--r--   0        0        0      973 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pyth_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26081 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
--rw-r--r--   0        0        0    54572 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/__init__.py
--rw-r--r--   0        0        0     6219 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_controller.py
--rw-r--r--   0        0        0     1357 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_helpers.py
--rw-r--r--   0        0        0     3447 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_model.py
--rw-r--r--   0        0        0     2772 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_view.py
--rw-r--r--   0        0        0    16935 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_prompt_toolkit.py
--rw-r--r--   0        0        0    55138 2023-04-10 00:09:07.453164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
--rw-r--r--   0        0        0  2879534 2023-04-10 00:09:07.473164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
--rw-r--r--   0        0        0   350260 2023-04-10 00:09:07.473164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
--rw-r--r--   0        0        0   607642 2023-04-10 00:09:07.477164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
--rw-r--r--   0        0        0    11988 2023-04-10 00:09:07.477164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
--rw-r--r--   0        0        0   667206 2023-04-10 00:09:07.481164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/tvl.png
--rw-r--r--   0        0        0   465754 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/__init__.py
--rw-r--r--   0        0        0    15437 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/dashboards_controller.py
--rw-r--r--   0        0        0    15983 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/stream/Forecasting.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/stream/__init__.py
--rw-r--r--   0        0        0    16808 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/stream/pages/Indicators.py
--rw-r--r--   0        0        0     5481 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/chains.ipynb
--rw-r--r--   0        0        0     6789 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/correlation.ipynb
--rw-r--r--   0        0        0    13852 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/forecast.ipynb
--rw-r--r--   0        0        0    10953 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/futures.ipynb
--rw-r--r--   0        0        0     9421 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/shortdata.ipynb
--rw-r--r--   0        0        0    15315 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/stocks.ipynb
--rw-r--r--   0        0        0     5091 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/decorators.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/__init__.py
--rw-r--r--   0        0        0    73682 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_controller.py
--rw-r--r--   0        0        0     2973 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_helpers.py
--rw-r--r--   0        0        0    13544 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_model.py
--rw-r--r--   0        0        0    16620 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_view.py
--rw-r--r--   0        0        0    20449 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/regression_model.py
--rw-r--r--   0        0        0     6739 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/regression_view.py
--rw-r--r--   0        0        0       77 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/__init__.py
--rw-r--r--   0        0        0    10230 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/alphavantage_model.py
--rw-r--r--   0        0        0    12075 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/alphavantage_view.py
--rw-r--r--   0        0        0     1614 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/commodity_model.py
--rw-r--r--   0        0        0     1561 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/commodity_view.py
--rw-r--r--   0        0        0      909 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
--rw-r--r--   0        0        0    21218 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/cpi.csv
--rw-r--r--   0        0        0    10355 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/harmonized_cpi.csv
--rw-r--r--   0        0        0    28404 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/econdb_model.py
--rw-r--r--   0        0        0     8013 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/econdb_view.py
--rw-r--r--   0        0        0    91589 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/economy_controller.py
--rw-r--r--   0        0        0     3436 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/economy_helpers.py
--rw-r--r--   0        0        0     1298 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finnhub_model.py
--rw-r--r--   0        0        0     2581 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finnhub_view.py
--rw-r--r--   0        0        0     7966 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finviz_model.py
--rw-r--r--   0        0        0     4600 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finviz_view.py
--rw-r--r--   0        0        0     9940 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/fred_model.py
--rw-r--r--   0        0        0     9117 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/fred_view.py
--rw-r--r--   0        0        0     6972 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/nasdaq_model.py
--rw-r--r--   0        0        0     3286 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/nasdaq_view.py
--rw-r--r--   0        0        0    38418 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/oecd_model.py
--rw-r--r--   0        0        0    26364 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/oecd_view.py
--rw-r--r--   0        0        0     3768 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/plot_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    28433 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1218 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/sdk_helpers.py
--rw-r--r--   0        0        0    12870 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/wsj_model.py
--rw-r--r--   0        0        0     4673 2023-04-10 00:09:07.485164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/wsj_view.py
--rw-r--r--   0        0        0    30415 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/yfinance_model.py
--rw-r--r--   0        0        0     5055 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/yfinance_view.py
--rw-r--r--   0        0        0      106 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/__init__.py
--rw-r--r--   0        0        0     4023 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/disc_controller.py
--rw-r--r--   0        0        0     2804 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/wsj_model.py
--rw-r--r--   0        0        0     1320 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/wsj_view.py
--rw-r--r--   0        0        0    21045 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/etf_controller.py
--rw-r--r--   0        0        0      450 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/etf_helper.py
--rw-r--r--   0        0        0   188615 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/etfs.csv
--rw-r--r--   0        0        0     2608 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/financedatabase_model.py
--rw-r--r--   0        0        0     3864 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/financedatabase_view.py
--rw-r--r--   0        0        0     1417 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/fmp_model.py
--rw-r--r--   0        0        0     3152 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/fmp_view.py
--rw-r--r--   0        0        0     4172 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/stockanalysis_model.py
--rw-r--r--   0        0        0     3941 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/stockanalysis_view.py
--rw-r--r--   0        0        0    51458 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     8025 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/featflags_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/__init__.py
--rw-r--r--   0        0        0    58622 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/corporate_spot_rates.csv
--rw-r--r--   0        0        0     9217 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ecb_model.py
--rw-r--r--   0        0        0     7096 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ecb_view.py
--rw-r--r--   0        0        0     5811 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/econdb_model.py
--rw-r--r--   0        0        0     7831 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/econdb_view.py
--rw-r--r--   0        0        0    56207 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fixedincome_controller.py
--rw-r--r--   0        0        0    37985 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fred_model.py
--rw-r--r--   0        0        0    51962 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fred_view.py
--rw-r--r--   0        0        0   227110 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ice_bofa_indices.csv
--rw-r--r--   0        0        0    10963 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/oecd_model.py
--rw-r--r--   0        0        0     3997 2023-04-10 00:09:07.489164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/oecd_view.py
--rw-r--r--   0        0        0     2174 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/yfinance_model.py
--rw-r--r--   0        0        0     1702 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/__init__.py
--rw-r--r--   0        0        0     1547 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/anom_model.py
--rw-r--r--   0        0        0     2962 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/anom_view.py
--rw-r--r--   0        0        0     4629 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoarima_model.py
--rw-r--r--   0        0        0     3933 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoarima_view.py
--rw-r--r--   0        0        0     4658 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoces_model.py
--rw-r--r--   0        0        0     3970 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoces_view.py
--rw-r--r--   0        0        0     4694 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoets_model.py
--rw-r--r--   0        0        0     3972 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoets_view.py
--rw-r--r--   0        0        0     7272 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoselect_model.py
--rw-r--r--   0        0        0     3938 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoselect_view.py
--rw-r--r--   0        0        0     5874 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/brnn_model.py
--rw-r--r--   0        0        0     6577 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/brnn_view.py
--rw-r--r--   0        0        0     5562 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/expo_model.py
--rw-r--r--   0        0        0     5038 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/expo_view.py
--rw-r--r--   0        0        0     2053 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast.ipynb
--rw-r--r--   0        0        0   121785 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_controller.py
--rw-r--r--   0        0        0    15471 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_model.py
--rw-r--r--   0        0        0     9034 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_view.py
--rw-r--r--   0        0        0    47334 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/helpers.py
--rw-r--r--   0        0        0     3405 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/linregr_model.py
--rw-r--r--   0        0        0     4760 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/linregr_view.py
--rw-r--r--   0        0        0     5013 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/mstl_model.py
--rw-r--r--   0        0        0     3861 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/mstl_view.py
--rw-r--r--   0        0        0     5896 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nbeats_model.py
--rw-r--r--   0        0        0     6396 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nbeats_view.py
--rw-r--r--   0        0        0     7561 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nhits_model.py
--rw-r--r--   0        0        0     7952 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nhits_view.py
--rw-r--r--   0        0        0     3007 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/regr_model.py
--rw-r--r--   0        0        0     4521 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/regr_view.py
--rw-r--r--   0        0        0     5030 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rnn_model.py
--rw-r--r--   0        0        0     5533 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rnn_view.py
--rw-r--r--   0        0        0     4340 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rwd_model.py
--rw-r--r--   0        0        0     3643 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rwd_view.py
--rw-r--r--   0        0        0     4709 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/seasonalnaive_model.py
--rw-r--r--   0        0        0     3879 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/seasonalnaive_view.py
--rw-r--r--   0        0        0     5790 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tcn_model.py
--rw-r--r--   0        0        0     6289 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tcn_view.py
--rw-r--r--   0        0        0     7249 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tft_model.py
--rw-r--r--   0        0        0     6520 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tft_view.py
--rw-r--r--   0        0        0     4928 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/theta_model.py
--rw-r--r--   0        0        0     4379 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/theta_view.py
--rw-r--r--   0        0        0     6321 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/trans_model.py
--rw-r--r--   0        0        0     6765 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/trans_view.py
--rw-r--r--   0        0        0    12580 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/whisper_model.py
--rw-r--r--   0        0        0     2935 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/whisper_utils.py
--rw-r--r--   0        0        0      122 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/__init__.py
--rw-r--r--   0        0        0     5077 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/av_model.py
--rw-r--r--   0        0        0     1458 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/av_view.py
--rw-r--r--   0        0        0     3281 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/av_forex_currencies.csv
--rw-r--r--   0        0        0     7847 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/polygon_tickers.csv
--rw-r--r--   0        0        0   419838 2023-04-10 00:09:07.493164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/yahoofinance_forex.json
--rw-r--r--   0        0        0    16492 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/forex_controller.py
--rw-r--r--   0        0        0     8211 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/forex_helper.py
--rw-r--r--   0        0        0      931 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/fxempire_model.py
--rw-r--r--   0        0        0     1471 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/fxempire_view.py
--rw-r--r--   0        0        0    17162 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_controller.py
--rw-r--r--   0        0        0    22592 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_model.py
--rw-r--r--   0        0        0    12856 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_view.py
--rw-r--r--   0        0        0     2349 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/polygon_model.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26168 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1446 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/technical_analysis/__init__.py
--rw-r--r--   0        0        0    35136 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/__init__.py
--rw-r--r--   0        0        0     2218 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/databento_view.py
--rw-r--r--   0        0        0     8903 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/futures_controller.py
--rw-r--r--   0        0        0      358 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/futures_helper.py
--rw-r--r--   0        0        0      964 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/sdk_helper.py
--rw-r--r--   0        0        0     4989 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/yfinance_model.py
--rw-r--r--   0        0        0     7379 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/yfinance_view.py
--rw-r--r--   0        0        0    13288 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helper_classes.py
--rw-r--r--   0        0        0    67647 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helper_funcs.py
--rw-r--r--   0        0        0     3212 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helpers_denomination.py
--rw-r--r--   0        0        0     9052 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/intro.json
--rw-r--r--   0        0        0    42551 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_controller.py
--rw-r--r--   0        0        0    80350 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_model.py
--rw-r--r--   0        0        0     1148 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_view.py
--rw-r--r--   0        0        0     5984 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/loggers.py
--rw-r--r--   0        0        0     1722 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/menu.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/custom/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/economy/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.497164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
--rw-r--r--   0        0        0     8528 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/futures/futures.csv
--rw-r--r--   0        0        0    60770 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/i18n/en.yml
--rw-r--r--   0        0        0     5831 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
--rw-r--r--   0        0        0       64 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
--rw-r--r--   0        0        0       87 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
--rw-r--r--   0        0        0      153 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
--rw-r--r--   0        0        0      119 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
--rw-r--r--   0        0        0      856 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
--rw-r--r--   0        0        0      802 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
--rw-r--r--   0        0        0     1192 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
--rw-r--r--   0        0        0      374 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
--rw-r--r--   0        0        0      168 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
--rw-r--r--   0        0        0     1229 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
--rw-r--r--   0        0        0     1533 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
--rw-r--r--   0        0        0      561 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
--rw-r--r--   0        0        0       87 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
--rw-r--r--   0        0        0      768 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
--rw-r--r--   0        0        0      154 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
--rw-r--r--   0        0        0      120 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
--rw-r--r--   0        0        0     1333 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
--rw-r--r--   0        0        0     2082 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
--rw-r--r--   0        0        0      155 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
--rw-r--r--   0        0        0       33 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
--rw-r--r--   0        0        0       38 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
--rw-r--r--   0        0        0      878 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
--rw-r--r--   0        0        0      749 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
--rw-r--r--   0        0        0      301 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
--rw-r--r--   0        0        0      176 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
--rw-r--r--   0        0        0      241 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
--rw-r--r--   0        0        0      108 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
--rw-r--r--   0        0        0      745 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
--rw-r--r--   0        0        0       62 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
--rw-r--r--   0        0        0      630 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
--rw-r--r--   0        0        0      611 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
--rw-r--r--   0        0        0      173 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
--rw-r--r--   0        0        0     1275 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
--rw-r--r--   0        0        0     1826 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
--rw-r--r--   0        0        0       98 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
--rw-r--r--   0        0        0      683 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
--rw-r--r--   0        0        0       67 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
--rw-r--r--   0        0        0       65 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
--rw-r--r--   0        0        0      151 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
--rw-r--r--   0        0        0       83 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
--rw-r--r--   0        0        0      113 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
--rw-r--r--   0        0        0      174 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
--rw-r--r--   0        0        0      158 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
--rw-r--r--   0        0        0      132 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
--rw-r--r--   0        0        0      102 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
--rw-r--r--   0        0        0      258 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
--rw-r--r--   0        0        0      255 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
--rw-r--r--   0        0        0     1513 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
--rw-r--r--   0        0        0      422 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
--rw-r--r--   0        0        0      251 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
--rw-r--r--   0        0        0      145 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
--rw-r--r--   0        0        0     1874 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
--rw-r--r--   0        0        0       44 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
--rw-r--r--   0        0        0       31 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
--rw-r--r--   0        0        0       31 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
--rw-r--r--   0        0        0      470 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
--rw-r--r--   0        0        0      276 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
--rw-r--r--   0        0        0      340 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
--rw-r--r--   0        0        0       91 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
--rw-r--r--   0        0        0      121 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
--rw-r--r--   0        0        0       82 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
--rw-r--r--   0        0        0      644 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
--rw-r--r--   0        0        0      170 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
--rw-r--r--   0        0        0      347 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
--rw-r--r--   0        0        0      717 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
--rw-r--r--   0        0        0       82 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
--rw-r--r--   0        0        0       65 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
--rw-r--r--   0        0        0       16 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
--rw-r--r--   0        0        0       46 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
--rw-r--r--   0        0        0     1072 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/models/hub_credentials.json
--rw-r--r--   0        0        0      380 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/models/local_credentials.json
--rw-r--r--   0        0        0    17970 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
--rw-r--r--   0        0        0    29757 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
--rw-r--r--   0        0        0      310 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/routines/routine_example.openbb
--rw-r--r--   0        0        0    22698 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/sources/openbb_default.json
--rw-r--r--   0        0        0     2332 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
--rw-r--r--   0        0        0     2354 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
--rw-r--r--   0        0        0     2341 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
--rw-r--r--   0        0        0     2316 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
--rw-r--r--   0        0        0     2316 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
--rw-r--r--   0        0        0     2346 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
--rw-r--r--   0        0        0     2336 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
--rw-r--r--   0        0        0     2346 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
--rw-r--r--   0        0        0     2307 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
--rw-r--r--   0        0        0     2309 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
--rw-r--r--   0        0        0     2329 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
--rw-r--r--   0        0        0     2353 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
--rw-r--r--   0        0        0     2360 2023-04-10 00:09:07.501164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
--rw-r--r--   0        0        0     2320 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
--rw-r--r--   0        0        0     2344 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
--rw-r--r--   0        0        0     2315 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
--rw-r--r--   0        0        0     2346 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
--rw-r--r--   0        0        0     2376 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
--rw-r--r--   0        0        0     2326 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Health.ini
--rw-r--r--   0        0        0     2307 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
--rw-r--r--   0        0        0     2320 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
--rw-r--r--   0        0        0     2324 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
--rw-r--r--   0        0        0     2334 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
--rw-r--r--   0        0        0     2324 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
--rw-r--r--   0        0        0     2313 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
--rw-r--r--   0        0        0     2341 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
--rw-r--r--   0        0        0     2296 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
--rw-r--r--   0        0        0     2367 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
--rw-r--r--   0        0        0     2342 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
--rw-r--r--   0        0        0     2361 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
--rw-r--r--   0        0        0     2351 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
--rw-r--r--   0        0        0     2336 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
--rw-r--r--   0        0        0     2322 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
--rw-r--r--   0        0        0     2310 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
--rw-r--r--   0        0        0     2326 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
--rw-r--r--   0        0        0     2341 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
--rw-r--r--   0        0        0     2299 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
--rw-r--r--   0        0        0     2316 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
--rw-r--r--   0        0        0     2342 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
--rw-r--r--   0        0        0     2381 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
--rw-r--r--   0        0        0     2314 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
--rw-r--r--   0        0        0    34473 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/template.ini
--rw-r--r--   0        0        0    34519 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/whales.ini
--rw-r--r--   0        0        0     2688 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/README.md
--rw-r--r--   0        0        0     4195 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
--rw-r--r--   0        0        0     4210 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
--rw-r--r--   0        0        0     3925 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
--rw-r--r--   0        0        0     4202 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
--rw-r--r--   0        0        0     4079 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/template.ini
--rwxr-xr-x   0        0        0      282 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
--rw-r--r--   0        0        0    21940 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
--rwxr-xr-x   0        0        0      315 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
--rwxr-xr-x   0        0        0      464 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
--rw-r--r--   0        0        0      413 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
--rwxr-xr-x   0        0        0      184 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
--rwxr-xr-x   0        0        0      364 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
--rw-r--r--   0        0        0      326 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
--rw-r--r--   0        0        0      193 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
--rw-r--r--   0        0        0      241 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
--rwxr-xr-x   0        0        0      335 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
--rw-r--r--   0        0        0      286 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
--rwxr-xr-x   0        0        0      167 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
--rw-r--r--   0        0        0      221 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
--rwxr-xr-x   0        0        0      255 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
--rwxr-xr-x   0        0        0      518 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
--rw-r--r--   0        0        0      302 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
--rwxr-xr-x   0        0        0      279 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
--rw-r--r--   0        0        0      316 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
--rw-r--r--   0        0        0      349 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
--rwxr-xr-x   0        0        0      295 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
--rwxr-xr-x   0        0        0      274 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
--rwxr-xr-x   0        0        0      328 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
--rwxr-xr-x   0        0        0      301 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
--rwxr-xr-x   0        0        0      212 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
--rwxr-xr-x   0        0        0      295 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
--rw-r--r--   0        0        0      337 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
--rw-r--r--   0        0        0      280 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
--rw-r--r--   0        0        0      246 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
--rw-r--r--   0        0        0      360 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
--rwxr-xr-x   0        0        0      222 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
--rwxr-xr-x   0        0        0      260 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
--rwxr-xr-x   0        0        0      197 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
--rwxr-xr-x   0        0        0      211 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
--rwxr-xr-x   0        0        0      201 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
--rwxr-xr-x   0        0        0      203 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
--rwxr-xr-x   0        0        0      179 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
--rwxr-xr-x   0        0        0      185 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
--rwxr-xr-x   0        0        0      187 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
--rwxr-xr-x   0        0        0      189 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
--rwxr-xr-x   0        0        0      189 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
--rwxr-xr-x   0        0        0      187 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
--rwxr-xr-x   0        0        0      185 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
--rwxr-xr-x   0        0        0      276 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
--rwxr-xr-x   0        0        0      272 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
--rwxr-xr-x   0        0        0      299 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
--rwxr-xr-x   0        0        0      293 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
--rwxr-xr-x   0        0        0      286 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
--rw-r--r--   0        0        0      209 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
--rwxr-xr-x   0        0        0      272 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
--rwxr-xr-x   0        0        0      675 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
--rwxr-xr-x   0        0        0      315 2023-04-10 00:09:07.505164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
--rw-r--r--   0        0        0   358460 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
--rw-r--r--   0        0        0      972 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
--rw-r--r--   0        0        0     2086 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
--rw-r--r--   0        0        0     2750 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0      203 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
--rw-r--r--   0        0        0      970 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
--rw-r--r--   0        0        0     2035 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.mplstyle
--rw-r--r--   0        0        0    24077 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0      202 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
--rw-r--r--   0        0        0     2607 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0      186 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
--rw-r--r--   0        0        0      144 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/__init__.py
--rw-r--r--   0        0        0    81373 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_fund_ID.csv
--rw-r--r--   0        0        0      834 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_model.py
--rw-r--r--   0        0        0     3941 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_view.py
--rw-r--r--   0        0        0     6535 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mstarpy_model.py
--rw-r--r--   0        0        0     7883 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mstarpy_view.py
--rw-r--r--   0        0        0    15141 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mutual_fund_controller.py
--rw-r--r--   0        0        0     6040 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mutual_funds_utils.py
--rw-r--r--   0        0        0    51025 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/parent_classes.py
--rw-r--r--   0        0        0       61 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/__init__.py
--rw-r--r--   0        0        0    15080 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/allocation_model.py
--rw-r--r--   0        0        0    12944 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/attribution_model.py
--rw-r--r--   0        0        0      417 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/__init__.py
--rw-r--r--   0        0        0     3214 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/bro_controller.py
--rw-r--r--   0        0        0     1121 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/brokers_helpers.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/__init__.py
--rw-r--r--   0        0        0     8211 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
--rw-r--r--   0        0        0     9561 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
--rw-r--r--   0        0        0     4495 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
--rw-r--r--   0        0        0     4666 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.509164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/__init__.py
--rw-r--r--   0        0        0    12789 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
--rw-r--r--   0        0        0    15571 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
--rw-r--r--   0        0        0    15670 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
--rw-r--r--   0        0        0     3894 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
--rw-r--r--   0        0        0     3002 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
--rw-r--r--   0        0        0     2482 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
--rw-r--r--   0        0        0    30861 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/metrics_model.py
--rw-r--r--   0        0        0    54979 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_controller.py
--rw-r--r--   0        0        0    39188 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_engine.py
--rw-r--r--   0        0        0     9643 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_helper.py
--rw-r--r--   0        0        0    60205 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_model.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/__init__.py
--rw-r--r--   0        0        0     5255 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
--rw-r--r--   0        0        0     2106 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
--rw-r--r--   0        0        0   120571 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
--rw-r--r--   0        0        0   155050 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
--rw-r--r--   0        0        0     2773 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
--rw-r--r--   0        0        0    13116 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
--rw-r--r--   0        0        0     5965 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
--rw-r--r--   0        0        0     5346 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
--rw-r--r--   0        0        0     4427 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
--rw-r--r--   0        0        0   138034 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
--rw-r--r--   0        0        0     8587 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
--rw-r--r--   0        0        0   103568 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_model.py
--rw-r--r--   0        0        0    24186 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_view.py
--rw-r--r--   0        0        0    11390 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/statics.py
--rw-r--r--   0        0        0    12009 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
--rw-r--r--   0        0        0    54944 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_view.py
--rw-r--r--   0        0        0     8433 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/statics.py
--rw-r--r--   0        0        0     2877 2023-04-10 00:09:07.513164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reporting.md
--rw-r--r--   0        0        0  1028287 2023-04-10 00:09:07.517164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
--rw-r--r--   0        0        0     2839 2023-04-10 00:09:07.517164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.517164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/__init__.py
--rw-r--r--   0        0        0      443 2023-04-10 00:09:07.517164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/data/crypto_tickers.csv
--rw-r--r--   0        0        0      437 2023-04-10 00:09:07.517164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/data/etf_tickers.csv
--rw-r--r--   0        0        0      222 2023-04-10 00:09:07.521164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/data/stocks_tickers.csv
--rw-r--r--   0        0        0     9716 2023-04-10 00:09:07.521164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/reports_controller.py
--rw-r--r--   0        0        0    12275 2023-04-10 00:09:07.521164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/reports_model.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.521164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/stored/.gitkeep
--rw-r--r--   0        0        0  1076317 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
--rw-r--r--   0        0        0     5214 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/OpenBB_reports_logo.png
--rw-r--r--   0        0        0    32298 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/crypto.ipynb
--rw-r--r--   0        0        0    22724 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/economy.ipynb
--rw-r--r--   0        0        0    39716 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/equity.ipynb
--rw-r--r--   0        0        0     9851 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/etf.ipynb
--rw-r--r--   0        0        0     2782 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/floppy-disc.png
--rw-r--r--   0        0        0     8557 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/forecast.ipynb
--rw-r--r--   0        0        0    17576 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/forex.ipynb
--rw-r--r--   0        0        0    14912 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/portfolio.ipynb
--rw-r--r--   0        0        0    11247 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widget_helpers.py
--rw-r--r--   0        0        0      205 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/card.j2
--rw-r--r--   0        0        0     3556 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/report.css
--rw-r--r--   0        0        0      474 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/report.j2
--rw-r--r--   0        0        0      119 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/row.j2
--rw-r--r--   0        0        0      896 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/style.css
--rw-r--r--   0        0        0     9967 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/rich_config.py
--rw-r--r--   0        0        0    30901 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/sdk.py
--rw-r--r--   0        0        0    28128 2023-04-10 00:09:07.525164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/settings_controller.py
--rw-r--r--   0        0        0     7105 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/sources_controller.py
--rw-r--r--   0        0        0      357 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/__init__.py
--rw-r--r--   0        0        0    10448 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_controller.py
--rw-r--r--   0        0        0     8126 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_model.py
--rw-r--r--   0        0        0     9046 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0    29872 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
--rw-r--r--   0        0        0     3541 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3761 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     1931 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/cboe_model.py
--rw-r--r--   0        0        0      969 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/cboe_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/__init__.py
--rw-r--r--   0        0        0    37655 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/ca_controller.py
--rw-r--r--   0        0        0     4871 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
--rw-r--r--   0        0        0     5785 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1328 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
--rw-r--r--   0        0        0     2679 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
--rw-r--r--   0        0        0     1539 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
--rw-r--r--   0        0        0    12381 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     5757 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     1690 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/polygon_model.py
--rw-r--r--   0        0        0     1379 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
--rw-r--r--   0        0        0     8073 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    10157 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/__init__.py
--rw-r--r--   0        0        0    20377 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
--rw-r--r--   0        0        0    10009 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
--rw-r--r--   0        0        0     7203 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
--rw-r--r--   0        0        0     1093 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
--rw-r--r--   0        0        0     1200 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
--rw-r--r--   0        0        0     1387 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
--rw-r--r--   0        0        0     4648 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
--rw-r--r--   0        0        0     6836 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
--rw-r--r--   0        0        0     3470 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
--rw-r--r--   0        0        0     1882 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
--rw-r--r--   0        0        0     1385 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
--rw-r--r--   0        0        0     5053 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
--rw-r--r--   0        0        0     9997 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
--rw-r--r--   0        0        0     1166 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
--rw-r--r--   0        0        0     3613 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
--rw-r--r--   0        0        0      668 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
--rw-r--r--   0        0        0     1271 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
--rw-r--r--   0        0        0     5740 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/databento_model.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/__init__.py
--rw-r--r--   0        0        0     4169 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/ark_model.py
--rw-r--r--   0        0        0     2589 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/ark_view.py
--rw-r--r--   0        0        0    31510 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/disc_controller.py
--rw-r--r--   0        0        0      483 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/disc_helpers.py
--rw-r--r--   0        0        0     2696 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fidelity_model.py
--rw-r--r--   0        0        0     2680 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fidelity_view.py
--rw-r--r--   0        0        0     4164 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finnhub_model.py
--rw-r--r--   0        0        0     2510 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finnhub_view.py
--rw-r--r--   0        0        0     1731 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finviz_model.py
--rw-r--r--   0        0        0     3084 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finviz_view.py
--rw-r--r--   0        0        0     2562 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fmp_view.py
--rw-r--r--   0        0        0     3051 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/nasdaq_model.py
--rw-r--r--   0        0        0     3406 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/nasdaq_view.py
--rw-r--r--   0        0        0     7080 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/seeking_alpha_model.py
--rw-r--r--   0        0        0     4803 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/seeking_alpha_view.py
--rw-r--r--   0        0        0     1120 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/shortinterest_model.py
--rw-r--r--   0        0        0     2566 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/shortinterest_view.py
--rw-r--r--   0        0        0     4113 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/yahoofinance_model.py
--rw-r--r--   0        0        0     5871 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/yahoofinance_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/__init__.py
--rw-r--r--   0        0        0    24082 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/av_model.py
--rw-r--r--   0        0        0    14910 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/av_view.py
--rw-r--r--   0        0        0    10834 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
--rw-r--r--   0        0        0     7680 2023-04-10 00:09:07.529164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
--rw-r--r--   0        0        0     1833 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
--rw-r--r--   0        0        0     2347 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
--rw-r--r--   0        0        0    14888 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
--rw-r--r--   0        0        0     4279 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
--rw-r--r--   0        0        0    44464 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
--rw-r--r--   0        0        0     1532 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
--rw-r--r--   0        0        0     1205 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
--rw-r--r--   0        0        0     2396 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
--rw-r--r--   0        0        0     4904 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
--rw-r--r--   0        0        0    81236 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
--rw-r--r--   0        0        0      266 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
--rw-r--r--   0        0        0     1389 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3518 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3419 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
--rw-r--r--   0        0        0     2484 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
--rw-r--r--   0        0        0    22210 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
--rw-r--r--   0        0        0    25688 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
--rw-r--r--   0        0        0     6417 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
--rw-r--r--   0        0        0    11855 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py
--rw-r--r--   0        0        0     1509 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py
--rw-r--r--   0        0        0     2217 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     1259 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     5391 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
--rw-r--r--   0        0        0     4361 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
--rw-r--r--   0        0        0     7593 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
--rw-r--r--   0        0        0    11162 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
--rw-r--r--   0        0        0     2059 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
--rw-r--r--   0        0        0    11829 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    14679 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/__init__.py
--rw-r--r--   0        0        0    18461 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/gov_controller.py
--rw-r--r--   0        0        0    15719 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/quiverquant_model.py
--rw-r--r--   0        0        0    21407 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/quiverquant_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/__init__.py
--rw-r--r--   0        0        0     2062 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/businessinsider_model.py
--rw-r--r--   0        0        0     5102 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/businessinsider_view.py
--rw-r--r--   0        0        0     1125 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/finviz_model.py
--rw-r--r--   0        0        0     1171 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/finviz_view.py
--rw-r--r--   0        0        0    32744 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/insider_controller.py
--rw-r--r--   0        0        0    87496 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/openinsider_model.py
--rw-r--r--   0        0        0     7695 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/openinsider_view.py
--rw-r--r--   0        0        0     4909 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/sdk_helper.py
--rw-r--r--   0        0        0    76085 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/mappings/Mic_Codes.csv
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/__init__.py
--rw-r--r--   0        0        0     1757 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/alphaquery_model.py
--rw-r--r--   0        0        0     1713 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/alphaquery_view.py
--rw-r--r--   0        0        0     1161 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/barchart_model.py
--rw-r--r--   0        0        0     1137 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/barchart_view.py
--rw-r--r--   0        0        0     1526 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/calculator_model.py
--rw-r--r--   0        0        0     2416 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/calculator_view.py
--rw-r--r--   0        0        0     2777 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/chartexchange_model.py
--rw-r--r--   0        0        0     3211 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/chartexchange_view.py
--rw-r--r--   0        0        0     2433 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/fdscanner_model.py
--rw-r--r--   0        0        0     1672 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/fdscanner_view.py
--rw-r--r--   0        0        0    21092 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_controller.py
--rw-r--r--   0        0        0     9884 2023-04-10 00:09:07.533164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_model.py
--rw-r--r--   0        0        0     3968 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_view.py
--rw-r--r--   0        0        0    10030 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/intrinio_model.py
--rw-r--r--   0        0        0     6101 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/intrinio_view.py
--rw-r--r--   0        0        0     7097 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/nasdaq_model.py
--rw-r--r--   0        0        0    22486 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/op_helpers.py
--rw-r--r--   0        0        0    52192 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_controller.py
--rw-r--r--   0        0        0    10568 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_sdk_helper.py
--rw-r--r--   0        0        0    14169 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/__init__.py
--rw-r--r--   0        0        0     5686 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/screener_controller.py
--rw-r--r--   0        0        0     9556 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/syncretism_model.py
--rw-r--r--   0        0        0     5566 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/syncretism_view.py
--rw-r--r--   0        0        0     8295 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/tradier_model.py
--rw-r--r--   0        0        0     2561 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/tradier_view.py
--rw-r--r--   0        0        0     7674 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/yfinance_model.py
--rw-r--r--   0        0        0    11615 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0     2260 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/beta_model.py
--rw-r--r--   0        0        0     2798 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/beta_view.py
--rw-r--r--   0        0        0     3187 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/factors_model.py
--rw-r--r--   0        0        0      687 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/factors_view.py
--rw-r--r--   0        0        0    38741 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0      447 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/research/__init__.py
--rw-r--r--   0        0        0     6218 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/research/res_controller.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/__init__.py
--rw-r--r--   0        0        0    46491 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/finviz_model.py
--rw-r--r--   0        0        0     6981 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/finviz_view.py
--rw-r--r--   0        0        0    21493 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_controller.py
--rw-r--r--   0        0        0      944 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_helper.py
--rw-r--r--   0        0        0     2562 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_view.py
--rw-r--r--   0        0        0    27077 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stock_statics.py
--rw-r--r--   0        0        0    27315 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_controller.py
--rw-r--r--   0        0        0    33068 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_helper.py
--rw-r--r--   0        0        0    10576 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_model.py
--rw-r--r--   0        0        0     1241 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finbrain_model.py
--rw-r--r--   0        0        0      644 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finbrain_view.py
--rw-r--r--   0        0        0      761 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finviz_model.py
--rw-r--r--   0        0        0     1229 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finviz_view.py
--rw-r--r--   0        0        0     1532 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/rsp_model.py
--rw-r--r--   0        0        0     2386 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/rsp_view.py
--rw-r--r--   0        0        0    63334 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     3260 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/tradingview_model.py
--rw-r--r--   0        0        0     1985 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/tradingview_view.py
--rw-r--r--   0        0        0      334 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/README.md
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/__init__.py
--rw-r--r--   0        0        0     5328 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/bursa_model.py
--rw-r--r--   0        0        0     2202 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/bursa_view.py
--rw-r--r--   0        0        0        0 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/data/__init__.py
--rw-r--r--   0        0        0    28098 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
--rw-r--r--   0        0        0     1466 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
--rw-r--r--   0        0        0     1378 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
--rw-r--r--   0        0        0    10137 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
--rw-r--r--   0        0        0      614 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
--rw-r--r--   0        0        0    42825 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/terminal_controller.py
--rw-r--r--   0        0        0    13888 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/terminal_helper.py
--rw-r--r--   0        0        0     3848 2023-04-10 00:09:07.537164 openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/thought_of_the_day.py
--rw-r--r--   0        0        0     5787 2023-04-10 00:09:09.317172 openbb_nightly-3.0.0rc1.dev20230410/pyproject.toml
--rw-r--r--   0        0        0      945 2023-04-10 00:09:07.541164 openbb_nightly-3.0.0rc1.dev20230410/terminal.py
--rw-r--r--   0        0        0     2293 2023-04-10 00:09:09.321172 openbb_nightly-3.0.0rc1.dev20230410/website/pypi.md
--rw-r--r--   0        0        0     7850 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc1.dev20230410/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-11 00:09:08.100305 openbb_nightly-3.0.0rc1.dev20230411/LICENSE
+-rw-r--r--   0        0        0    18588 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/SDK_README.md
+-rw-r--r--   0        0        0      243 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/__init__.py
+-rw-r--r--   0        0        0    19834 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_controller.py
+-rw-r--r--   0        0        0     3382 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_model.py
+-rw-r--r--   0        0        0      612 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/__init__.py
+-rw-r--r--   0        0        0     3131 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/alt_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/__init__.py
+-rw-r--r--   0        0        0     1881 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/countries.txt
+-rw-r--r--   0        0        0     9347 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_controller.py
+-rw-r--r--   0        0        0     5387 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_model.py
+-rw-r--r--   0        0        0     8586 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_view.py
+-rw-r--r--   0        0        0     1070 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/hackernews_model.py
+-rw-r--r--   0        0        0     1087 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/hackernews_view.py
+-rw-r--r--   0        0        0     6752 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/github_model.py
+-rw-r--r--   0        0        0     3968 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/github_view.py
+-rw-r--r--   0        0        0     8656 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/oss_controller.py
+-rw-r--r--   0        0        0     4437 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/runa_model.py
+-rw-r--r--   0        0        0     4018 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/runa_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/__init__.py
+-rw-r--r--   0        0        0     9030 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/landRegistry_model.py
+-rw-r--r--   0        0        0     3309 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/landRegistry_view.py
+-rw-r--r--   0        0        0     8108 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/realestate_controller.py
+-rw-r--r--   0        0        0     2718 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/base_helpers.py
+-rw-r--r--   0        0        0       93 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0     1198 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     4394 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1335 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     1861 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3329 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/google_model.py
+-rw-r--r--   0        0        0     7118 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/google_view.py
+-rw-r--r--   0        0        0     5524 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
+-rw-r--r--   0        0        0    18297 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_model.py
+-rw-r--r--   0        0        0    10206 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_view.py
+-rw-r--r--   0        0        0     3239 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
+-rw-r--r--   0        0        0     2898 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
+-rw-r--r--   0        0        0     6160 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/twitter_model.py
+-rw-r--r--   0        0        0     5870 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/twitter_view.py
+-rw-r--r--   0        0        0     4142 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/common_model.py
+-rw-r--r--   0        0        0     3634 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/feedparser_model.py
+-rw-r--r--   0        0        0     1242 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/feedparser_view.py
+-rw-r--r--   0        0        0     2639 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/newsapi_model.py
+-rw-r--r--   0        0        0     1465 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/newsapi_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    19923 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0    32308 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/qa_view.py
+-rw-r--r--   0        0        0     3226 2023-04-11 00:09:08.260308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/rolling_model.py
+-rw-r--r--   0        0        0    10790 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/rolling_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     2977 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/custom_indicators_model.py
+-rw-r--r--   0        0        0     4272 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/custom_indicators_view.py
+-rw-r--r--   0        0        0     6427 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/momentum_model.py
+-rw-r--r--   0        0        0    10556 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/momentum_view.py
+-rw-r--r--   0        0        0     4179 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/overlap_model.py
+-rw-r--r--   0        0        0     4361 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/overlap_view.py
+-rw-r--r--   0        0        0     1453 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/ta_helpers.py
+-rw-r--r--   0        0        0     1819 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/trend_indicators_model.py
+-rw-r--r--   0        0        0     2621 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/trend_indicators_view.py
+-rw-r--r--   0        0        0    19962 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volatility_model.py
+-rw-r--r--   0        0        0    10008 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volatility_view.py
+-rw-r--r--   0        0        0     2614 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volume_model.py
+-rw-r--r--   0        0        0     3806 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volume_view.py
+-rw-r--r--   0        0        0     5813 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/ultima_newsmonitor_model.py
+-rw-r--r--   0        0        0     3886 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/ultima_newsmonitor_view.py
+-rw-r--r--   0        0        0     2634 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/config_terminal.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/__init__.py
+-rw-r--r--   0        0        0     9829 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/completer/choices.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/config/__init__.py
+-rw-r--r--   0        0        0      927 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/config/paths.py
+-rw-r--r--   0        0        0     2650 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/config/paths_helper.py
+-rw-r--r--   0        0        0     9162 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/integration_tests/README.md
+-rw-r--r--   0        0        0    21758 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/integration_tests/integration_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/__init__.py
+-rw-r--r--   0        0        0     3848 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/log_sender.py
+-rw-r--r--   0        0        0     3744 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/logging_clock.py
+-rw-r--r--   0        0        0     3495 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/s3_sender.py
+-rw-r--r--   0        0        0      166 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/constants.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/__init__.py
+-rw-r--r--   0        0        0      524 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/common.py
+-rw-r--r--   0        0        0      525 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/custom_logger.py
+-rw-r--r--   0        0        0      979 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/directories.py
+-rw-r--r--   0        0        0      841 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/expired_files.py
+-rw-r--r--   0        0        0     4896 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     6058 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4166 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/settings.py
+-rw-r--r--   0        0        0     1621 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/settings_logger.py
+-rw-r--r--   0        0        0      396 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/user_logger.py
+-rw-r--r--   0        0        0      627 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/__init__.py
+-rw-r--r--   0        0        0     1221 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/base_model.py
+-rw-r--r--   0        0        0      818 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/credentials_model.py
+-rw-r--r--   0        0        0     4154 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/preferences_model.py
+-rw-r--r--   0        0        0     1817 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/profile_model.py
+-rw-r--r--   0        0        0     1230 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/sources_model.py
+-rw-r--r--   0        0        0     1753 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/system_model.py
+-rw-r--r--   0        0        0      562 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/user_model.py
+-rw-r--r--   0        0        0      200 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/__init__.py
+-rw-r--r--   0        0        0   418780 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/assets/Terminal_icon.png
+-rw-r--r--   0        0        0      727 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/assets/icon.png
+-rw-r--r--   0        0        0    14854 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/backend.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/config/__init__.py
+-rw-r--r--   0        0        0     7156 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/config/openbb_styles.py
+-rw-r--r--   0        0        0     3073 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/no_import.py
+-rw-r--r--   0        0        0     1261 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/old_table.html
+-rw-r--r--   0        0        0     7732 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly.html
+-rw-r--r--   0        0        0    62751 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_helper.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.264308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     6724 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/base.py
+-rw-r--r--   0        0        0    11358 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8016 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    15173 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3361 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5683 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6868 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3429 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    20644 2023-04-11 00:09:08.268308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0   704570 2023-04-11 00:09:08.272308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/table.html
+-rw-r--r--   0        0        0    11182 2023-04-11 00:09:08.272308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/bar_menus.js
+-rw-r--r--   0        0        0   289624 2023-04-11 00:09:08.272308 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf
+-rw-r--r--   0        0        0   286320 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf
+-rw-r--r--   0        0        0    25671 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/style.css
+-rw-r--r--   0        0        0      151 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/table.css
+-rw-r--r--   0        0        0    16655 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/helpers.js
+-rw-r--r--   0        0        0    13012 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/main.js
+-rw-r--r--   0        0        0     3255 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/main_table.js
+-rw-r--r--   0        0        0    24525 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/popups.js
+-rw-r--r--   0        0        0     7747 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/scripts/sdk_audit.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/__init__.py
+-rw-r--r--   0        0        0      450 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
+-rw-r--r--   0        0        0    24088 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
+-rw-r--r--   0        0        0     1513 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
+-rw-r--r--   0        0        0     2365 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
+-rw-r--r--   0        0        0     5128 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
+-rw-r--r--   0        0        0    18447 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
+-rw-r--r--   0        0        0      761 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/__init__.py
+-rw-r--r--   0        0        0     4308 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/alt_sdk_model.py
+-rw-r--r--   0        0        0    42910 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/crypto_sdk_model.py
+-rw-r--r--   0        0        0     4497 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
+-rw-r--r--   0        0        0     7975 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/economy_sdk_model.py
+-rw-r--r--   0        0        0     2496 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/etf_sdk_model.py
+-rw-r--r--   0        0        0     3515 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
+-rw-r--r--   0        0        0     8550 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/forecast_sdk_model.py
+-rw-r--r--   0        0        0     4386 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/forex_sdk_model.py
+-rw-r--r--   0        0        0     1530 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/funds_sdk_model.py
+-rw-r--r--   0        0        0     1067 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/futures_sdk_model.py
+-rw-r--r--   0        0        0     3638 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/keys_sdk_model.py
+-rw-r--r--   0        0        0    10046 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
+-rw-r--r--   0        0        0     4603 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/qa_sdk_model.py
+-rw-r--r--   0        0        0    32674 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/stocks_sdk_model.py
+-rw-r--r--   0        0        0     7229 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/ta_sdk_model.py
+-rw-r--r--   0        0        0    11508 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/sdk_helpers.py
+-rw-r--r--   0        0        0    19813 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/sdk_init.py
+-rw-r--r--   0        0        0    43994 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map.csv
+-rw-r--r--   0        0        0     2801 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map_forecasting.csv
+-rw-r--r--   0        0        0     1301 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map_optimization.csv
+-rw-r--r--   0        0        0     7118 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trailmap.py
+-rw-r--r--   0        0        0     1017 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/banner.txt
+-rw-r--r--   0        0        0      485 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/constants.py
+-rw-r--r--   0        0        0     1000 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/current_system.py
+-rw-r--r--   0        0        0     4095 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/current_user.py
+-rw-r--r--   0        0        0     1147 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/env_handler.py
+-rw-r--r--   0        0        0    20779 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/hub_model.py
+-rw-r--r--   0        0        0     5477 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/local_model.py
+-rw-r--r--   0        0        0     3097 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/sdk_session.py
+-rw-r--r--   0        0        0     2913 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/session_controller.py
+-rw-r--r--   0        0        0     4656 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/session_model.py
+-rw-r--r--   0        0        0     2834 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/sources_handler.py
+-rw-r--r--   0        0        0     1551 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/utils.py
+-rw-r--r--   0        0        0     3011 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sources/utils.py
+-rw-r--r--   0        0        0      199 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/README.md
+-rw-r--r--   0        0        0       84 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/__init__.py
+-rw-r--r--   0        0        0     5303 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/coinbase_helpers.py
+-rw-r--r--   0        0        0     2147 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
+-rw-r--r--   0        0        0    19295 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_controller.py
+-rw-r--r--   0        0        0     4481 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_models.py
+-rw-r--r--   0        0        0     1785 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_views.py
+-rw-r--r--   0        0        0    30339 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
+-rw-r--r--   0        0        0      949 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/README.md
+-rw-r--r--   0        0        0     7341 2023-04-11 00:09:08.276309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
+-rw-r--r--   0        0        0     2436 2023-04-11 00:09:08.280309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
+-rw-r--r--   0        0        0     4813 2023-04-11 00:09:08.280309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coingecko_categories.json
+-rw-r--r--   0        0        0   954385 2023-04-11 00:09:08.280309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coingecko_coins.json
+-rw-r--r--   0        0        0  2245016 2023-04-11 00:09:08.288309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
+-rw-r--r--   0        0        0    31307 2023-04-11 00:09:08.288309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/defillama_dapps.json
+-rw-r--r--   0        0        0   107203 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/erc20_coins.json
+-rw-r--r--   0        0        0     7255 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/finbrain_coins.json
+-rw-r--r--   0        0        0   222978 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/santiment_slugs.json
+-rw-r--r--   0        0        0   300253 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
+-rw-r--r--   0        0        0     4951 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/dataframe_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/__init__.py
+-rw-r--r--   0        0        0     4537 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/coindix_model.py
+-rw-r--r--   0        0        0     2720 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/coindix_view.py
+-rw-r--r--   0        0        0     2483 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
+-rw-r--r--   0        0        0     1994 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
+-rw-r--r--   0        0        0    31284 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/defi_controller.py
+-rw-r--r--   0        0        0     8918 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/graph_model.py
+-rw-r--r--   0        0        0     7165 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/graph_view.py
+-rw-r--r--   0        0        0     5005 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/llama_model.py
+-rw-r--r--   0        0        0     5827 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/llama_view.py
+-rw-r--r--   0        0        0     1808 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/smartstake_model.py
+-rw-r--r--   0        0        0     3110 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/smartstake_view.py
+-rw-r--r--   0        0        0     2882 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/substack_model.py
+-rw-r--r--   0        0        0     1090 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/substack_view.py
+-rw-r--r--   0        0        0     1947 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
+-rw-r--r--   0        0        0     2699 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
+-rw-r--r--   0        0        0     9734 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
+-rw-r--r--   0        0        0     8022 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/__init__.py
+-rw-r--r--   0        0        0     2317 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
+-rw-r--r--   0        0        0     1620 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
+-rw-r--r--   0        0        0     2116 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
+-rw-r--r--   0        0        0     1936 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
+-rw-r--r--   0        0        0     7614 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
+-rw-r--r--   0        0        0     5045 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
+-rw-r--r--   0        0        0    21019 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    10833 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
+-rw-r--r--   0        0        0     6352 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
+-rw-r--r--   0        0        0     1095 2023-04-11 00:09:08.292309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/__init__.py
+-rw-r--r--   0        0        0     7483 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
+-rw-r--r--   0        0        0     3009 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
+-rw-r--r--   0        0        0     3188 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
+-rw-r--r--   0        0        0     2840 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
+-rw-r--r--   0        0        0     6439 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
+-rw-r--r--   0        0        0     4134 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
+-rw-r--r--   0        0        0     6587 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
+-rw-r--r--   0        0        0     6638 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
+-rw-r--r--   0        0        0    15062 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
+-rw-r--r--   0        0        0     9133 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
+-rw-r--r--   0        0        0     2332 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
+-rw-r--r--   0        0        0    64101 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
+-rw-r--r--   0        0        0     1850 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
+-rw-r--r--   0        0        0     4333 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
+-rw-r--r--   0        0        0    15044 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
+-rw-r--r--   0        0        0    11237 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
+-rw-r--r--   0        0        0    24480 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
+-rw-r--r--   0        0        0    22260 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
+-rw-r--r--   0        0        0    25887 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
+-rw-r--r--   0        0        0     8762 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
+-rw-r--r--   0        0        0     3076 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
+-rw-r--r--   0        0        0     2070 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
+-rw-r--r--   0        0        0     2508 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
+-rw-r--r--   0        0        0     6001 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
+-rw-r--r--   0        0        0     3474 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/__init__.py
+-rw-r--r--   0        0        0     5562 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nft_controller.py
+-rw-r--r--   0        0        0     1664 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
+-rw-r--r--   0        0        0     4495 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
+-rw-r--r--   0        0        0     2895 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/opensea_model.py
+-rw-r--r--   0        0        0     1289 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/opensea_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/__init__.py
+-rw-r--r--   0        0        0    21848 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
+-rw-r--r--   0        0        0    11444 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
+-rw-r--r--   0        0        0     3393 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
+-rw-r--r--   0        0        0     4733 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
+-rw-r--r--   0        0        0     1840 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
+-rw-r--r--   0        0        0     1266 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
+-rw-r--r--   0        0        0    15974 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
+-rw-r--r--   0        0        0    10572 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
+-rw-r--r--   0        0        0    53494 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
+-rw-r--r--   0        0        0     5938 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/shroom_model.py
+-rw-r--r--   0        0        0     5144 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/shroom_view.py
+-rw-r--r--   0        0        0     4772 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
+-rw-r--r--   0        0        0     2088 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/__init__.py
+-rw-r--r--   0        0        0     2274 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
+-rw-r--r--   0        0        0     2664 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
+-rw-r--r--   0        0        0     1464 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinbase_model.py
+-rw-r--r--   0        0        0     1342 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinbase_view.py
+-rw-r--r--   0        0        0    11841 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
+-rw-r--r--   0        0        0     9646 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
+-rw-r--r--   0        0        0     6776 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
+-rw-r--r--   0        0        0     2278 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
+-rw-r--r--   0        0        0     1100 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/glassnode_model.py
+-rw-r--r--   0        0        0     4677 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/glassnode_view.py
+-rw-r--r--   0        0        0     5936 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/loanscan_model.py
+-rw-r--r--   0        0        0     3279 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/loanscan_view.py
+-rw-r--r--   0        0        0    55381 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/overview_controller.py
+-rw-r--r--   0        0        0    13641 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
+-rw-r--r--   0        0        0    21320 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
+-rw-r--r--   0        0        0     5346 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/rekt_model.py
+-rw-r--r--   0        0        0     2253 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/rekt_view.py
+-rw-r--r--   0        0        0     2042 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
+-rw-r--r--   0        0        0     7167 2023-04-11 00:09:08.296309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
+-rw-r--r--   0        0        0     3126 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
+-rw-r--r--   0        0        0     6708 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
+-rw-r--r--   0        0        0     3480 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
+-rw-r--r--   0        0        0     7635 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
+-rw-r--r--   0        0        0     5693 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pyth_model.py
+-rw-r--r--   0        0        0      973 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pyth_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26081 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    54572 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/__init__.py
+-rw-r--r--   0        0        0     6219 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_controller.py
+-rw-r--r--   0        0        0     1357 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_helpers.py
+-rw-r--r--   0        0        0     3447 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_model.py
+-rw-r--r--   0        0        0     2772 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_view.py
+-rw-r--r--   0        0        0    16935 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_prompt_toolkit.py
+-rw-r--r--   0        0        0    55138 2023-04-11 00:09:08.300309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
+-rw-r--r--   0        0        0  2879534 2023-04-11 00:09:08.316310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
+-rw-r--r--   0        0        0   350260 2023-04-11 00:09:08.320309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
+-rw-r--r--   0        0        0   607642 2023-04-11 00:09:08.320309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
+-rw-r--r--   0        0        0    11988 2023-04-11 00:09:08.320309 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
+-rw-r--r--   0        0        0   667206 2023-04-11 00:09:08.324310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/tvl.png
+-rw-r--r--   0        0        0   465754 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/__init__.py
+-rw-r--r--   0        0        0    15437 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/dashboards_controller.py
+-rw-r--r--   0        0        0    15983 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/stream/Forecasting.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/stream/__init__.py
+-rw-r--r--   0        0        0    16808 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/stream/pages/Indicators.py
+-rw-r--r--   0        0        0     5481 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/chains.ipynb
+-rw-r--r--   0        0        0     6789 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/correlation.ipynb
+-rw-r--r--   0        0        0    13852 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/forecast.ipynb
+-rw-r--r--   0        0        0    10953 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/futures.ipynb
+-rw-r--r--   0        0        0     9421 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/shortdata.ipynb
+-rw-r--r--   0        0        0    15315 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/stocks.ipynb
+-rw-r--r--   0        0        0     5091 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/decorators.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/__init__.py
+-rw-r--r--   0        0        0    73682 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_controller.py
+-rw-r--r--   0        0        0     2973 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_helpers.py
+-rw-r--r--   0        0        0    13544 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_model.py
+-rw-r--r--   0        0        0    16620 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_view.py
+-rw-r--r--   0        0        0    20449 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/regression_model.py
+-rw-r--r--   0        0        0     6739 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/regression_view.py
+-rw-r--r--   0        0        0       77 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/__init__.py
+-rw-r--r--   0        0        0    10230 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/alphavantage_model.py
+-rw-r--r--   0        0        0    12075 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/alphavantage_view.py
+-rw-r--r--   0        0        0     1614 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/commodity_model.py
+-rw-r--r--   0        0        0     1561 2023-04-11 00:09:08.328310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/commodity_view.py
+-rw-r--r--   0        0        0      909 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
+-rw-r--r--   0        0        0    21218 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/cpi.csv
+-rw-r--r--   0        0        0    10355 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/harmonized_cpi.csv
+-rw-r--r--   0        0        0    28404 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/econdb_model.py
+-rw-r--r--   0        0        0     8013 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/econdb_view.py
+-rw-r--r--   0        0        0    91589 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/economy_controller.py
+-rw-r--r--   0        0        0     3436 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/economy_helpers.py
+-rw-r--r--   0        0        0     1298 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finnhub_model.py
+-rw-r--r--   0        0        0     2581 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finnhub_view.py
+-rw-r--r--   0        0        0     7966 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finviz_model.py
+-rw-r--r--   0        0        0     4600 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finviz_view.py
+-rw-r--r--   0        0        0     9940 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/fred_model.py
+-rw-r--r--   0        0        0     9117 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/fred_view.py
+-rw-r--r--   0        0        0     6972 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/nasdaq_model.py
+-rw-r--r--   0        0        0     3286 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/nasdaq_view.py
+-rw-r--r--   0        0        0    38418 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/oecd_model.py
+-rw-r--r--   0        0        0    26364 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/oecd_view.py
+-rw-r--r--   0        0        0     3768 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/plot_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    28433 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1218 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/sdk_helpers.py
+-rw-r--r--   0        0        0    12870 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/wsj_model.py
+-rw-r--r--   0        0        0     4673 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/wsj_view.py
+-rw-r--r--   0        0        0    30415 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/yfinance_model.py
+-rw-r--r--   0        0        0     5055 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/yfinance_view.py
+-rw-r--r--   0        0        0      106 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/__init__.py
+-rw-r--r--   0        0        0     4023 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/disc_controller.py
+-rw-r--r--   0        0        0     2804 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/wsj_model.py
+-rw-r--r--   0        0        0     1320 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/wsj_view.py
+-rw-r--r--   0        0        0    21045 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/etf_controller.py
+-rw-r--r--   0        0        0      450 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/etf_helper.py
+-rw-r--r--   0        0        0   188615 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/etfs.csv
+-rw-r--r--   0        0        0     2608 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/financedatabase_model.py
+-rw-r--r--   0        0        0     3864 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/financedatabase_view.py
+-rw-r--r--   0        0        0     1417 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/fmp_model.py
+-rw-r--r--   0        0        0     3152 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/fmp_view.py
+-rw-r--r--   0        0        0     4172 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/stockanalysis_model.py
+-rw-r--r--   0        0        0     3941 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/stockanalysis_view.py
+-rw-r--r--   0        0        0    51458 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     8025 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/featflags_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/__init__.py
+-rw-r--r--   0        0        0    58622 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2023-04-11 00:09:08.332310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/corporate_spot_rates.csv
+-rw-r--r--   0        0        0     9217 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     7096 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ecb_view.py
+-rw-r--r--   0        0        0     5811 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/econdb_model.py
+-rw-r--r--   0        0        0     7831 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/econdb_view.py
+-rw-r--r--   0        0        0    56207 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0    37985 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fred_model.py
+-rw-r--r--   0        0        0    51962 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fred_view.py
+-rw-r--r--   0        0        0   227110 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ice_bofa_indices.csv
+-rw-r--r--   0        0        0    10963 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/oecd_model.py
+-rw-r--r--   0        0        0     3997 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/oecd_view.py
+-rw-r--r--   0        0        0     2174 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/yfinance_model.py
+-rw-r--r--   0        0        0     1702 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/__init__.py
+-rw-r--r--   0        0        0     1547 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/anom_model.py
+-rw-r--r--   0        0        0     2962 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/anom_view.py
+-rw-r--r--   0        0        0     4629 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoarima_model.py
+-rw-r--r--   0        0        0     3933 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoarima_view.py
+-rw-r--r--   0        0        0     4658 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoces_model.py
+-rw-r--r--   0        0        0     3970 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoces_view.py
+-rw-r--r--   0        0        0     4694 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoets_model.py
+-rw-r--r--   0        0        0     3972 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoets_view.py
+-rw-r--r--   0        0        0     7272 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoselect_model.py
+-rw-r--r--   0        0        0     3938 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoselect_view.py
+-rw-r--r--   0        0        0     5874 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/brnn_model.py
+-rw-r--r--   0        0        0     6577 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/brnn_view.py
+-rw-r--r--   0        0        0     5562 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/expo_model.py
+-rw-r--r--   0        0        0     5038 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/expo_view.py
+-rw-r--r--   0        0        0     2053 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast.ipynb
+-rw-r--r--   0        0        0   121785 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_controller.py
+-rw-r--r--   0        0        0    15471 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_model.py
+-rw-r--r--   0        0        0     9034 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_view.py
+-rw-r--r--   0        0        0    47334 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/helpers.py
+-rw-r--r--   0        0        0     3405 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/linregr_model.py
+-rw-r--r--   0        0        0     4760 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/linregr_view.py
+-rw-r--r--   0        0        0     5013 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/mstl_model.py
+-rw-r--r--   0        0        0     3861 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/mstl_view.py
+-rw-r--r--   0        0        0     5896 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nbeats_model.py
+-rw-r--r--   0        0        0     6396 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nbeats_view.py
+-rw-r--r--   0        0        0     7561 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nhits_model.py
+-rw-r--r--   0        0        0     7952 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nhits_view.py
+-rw-r--r--   0        0        0     3007 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/regr_model.py
+-rw-r--r--   0        0        0     4521 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/regr_view.py
+-rw-r--r--   0        0        0     5030 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rnn_model.py
+-rw-r--r--   0        0        0     5533 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rnn_view.py
+-rw-r--r--   0        0        0     4340 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rwd_model.py
+-rw-r--r--   0        0        0     3643 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rwd_view.py
+-rw-r--r--   0        0        0     4709 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/seasonalnaive_model.py
+-rw-r--r--   0        0        0     3879 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/seasonalnaive_view.py
+-rw-r--r--   0        0        0     5790 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tcn_model.py
+-rw-r--r--   0        0        0     6289 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tcn_view.py
+-rw-r--r--   0        0        0     7249 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tft_model.py
+-rw-r--r--   0        0        0     6520 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tft_view.py
+-rw-r--r--   0        0        0     4928 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/theta_model.py
+-rw-r--r--   0        0        0     4379 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/theta_view.py
+-rw-r--r--   0        0        0     6321 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/trans_model.py
+-rw-r--r--   0        0        0     6765 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/trans_view.py
+-rw-r--r--   0        0        0    12580 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/whisper_model.py
+-rw-r--r--   0        0        0     2935 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/whisper_utils.py
+-rw-r--r--   0        0        0      122 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.336310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/__init__.py
+-rw-r--r--   0        0        0     5077 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/av_model.py
+-rw-r--r--   0        0        0     1458 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/av_view.py
+-rw-r--r--   0        0        0     3281 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/av_forex_currencies.csv
+-rw-r--r--   0        0        0     7847 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/polygon_tickers.csv
+-rw-r--r--   0        0        0   419838 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/yahoofinance_forex.json
+-rw-r--r--   0        0        0    16492 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/forex_controller.py
+-rw-r--r--   0        0        0     8211 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/forex_helper.py
+-rw-r--r--   0        0        0      931 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/fxempire_model.py
+-rw-r--r--   0        0        0     1471 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/fxempire_view.py
+-rw-r--r--   0        0        0    17162 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_controller.py
+-rw-r--r--   0        0        0    22592 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_model.py
+-rw-r--r--   0        0        0    12856 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_view.py
+-rw-r--r--   0        0        0     2349 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/polygon_model.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26168 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1446 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    35136 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/__init__.py
+-rw-r--r--   0        0        0     2218 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/databento_view.py
+-rw-r--r--   0        0        0     8903 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/futures_controller.py
+-rw-r--r--   0        0        0      358 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/futures_helper.py
+-rw-r--r--   0        0        0      964 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/sdk_helper.py
+-rw-r--r--   0        0        0     4989 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/yfinance_model.py
+-rw-r--r--   0        0        0     7379 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/yfinance_view.py
+-rw-r--r--   0        0        0    13288 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helper_classes.py
+-rw-r--r--   0        0        0    67647 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helper_funcs.py
+-rw-r--r--   0        0        0     3212 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helpers_denomination.py
+-rw-r--r--   0        0        0     9052 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/intro.json
+-rw-r--r--   0        0        0    42551 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_controller.py
+-rw-r--r--   0        0        0    80350 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_model.py
+-rw-r--r--   0        0        0     1148 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_view.py
+-rw-r--r--   0        0        0     5984 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/loggers.py
+-rw-r--r--   0        0        0     1722 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/menu.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/custom/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/economy/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.340310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0     8528 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/futures/futures.csv
+-rw-r--r--   0        0        0    60770 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/i18n/en.yml
+-rw-r--r--   0        0        0     5831 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
+-rw-r--r--   0        0        0       64 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
+-rw-r--r--   0        0        0       87 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_covid.openbb
+-rw-r--r--   0        0        0      153 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_oss.openbb
+-rw-r--r--   0        0        0      119 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt_realestate.openbb
+-rw-r--r--   0        0        0      856 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
+-rw-r--r--   0        0        0      802 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb
+-rw-r--r--   0        0        0     1192 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb
+-rw-r--r--   0        0        0      374 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_disc.openbb
+-rw-r--r--   0        0        0      168 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_nft.openbb
+-rw-r--r--   0        0        0     1229 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb
+-rw-r--r--   0        0        0     1533 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb
+-rw-r--r--   0        0        0      561 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb
+-rw-r--r--   0        0        0       87 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_shroom.openbb
+-rw-r--r--   0        0        0      768 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb
+-rw-r--r--   0        0        0      154 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_tools.openbb
+-rw-r--r--   0        0        0      120 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards_base.openbb
+-rw-r--r--   0        0        0     1333 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb
+-rw-r--r--   0        0        0     2082 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
+-rw-r--r--   0        0        0      155 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
+-rw-r--r--   0        0        0       33 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ca.openbb
+-rw-r--r--   0        0        0       38 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_disc.openbb
+-rw-r--r--   0        0        0      878 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb
+-rw-r--r--   0        0        0      749 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
+-rw-r--r--   0        0        0      301 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
+-rw-r--r--   0        0        0      176 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast_advanced.openbb
+-rw-r--r--   0        0        0      241 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_base.openbb
+-rw-r--r--   0        0        0      108 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_load.openbb
+-rw-r--r--   0        0        0      745 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb
+-rw-r--r--   0        0        0       62 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda_base.openbb
+-rw-r--r--   0        0        0      630 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb
+-rw-r--r--   0        0        0      611 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb
+-rw-r--r--   0        0        0      173 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
+-rw-r--r--   0        0        0     1275 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb
+-rw-r--r--   0        0        0     1826 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
+-rw-r--r--   0        0        0       98 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_boolean_args.openbb
+-rw-r--r--   0        0        0      683 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb
+-rw-r--r--   0        0        0       67 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_base.openbb
+-rw-r--r--   0        0        0       65 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_crypto.openbb
+-rw-r--r--   0        0        0      151 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_economy.openbb
+-rw-r--r--   0        0        0       83 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_equity.openbb
+-rw-r--r--   0        0        0      113 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_etf.openbb
+-rw-r--r--   0        0        0      174 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forecast.openbb
+-rw-r--r--   0        0        0      158 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_forex.openbb
+-rw-r--r--   0        0        0      132 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_portfolio.openbb
+-rw-r--r--   0        0        0      102 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports_run.openbb
+-rw-r--r--   0        0        0      258 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
+-rw-r--r--   0        0        0      255 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ba.openbb
+-rw-r--r--   0        0        0     1513 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb
+-rw-r--r--   0        0        0      422 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ca.openbb
+-rw-r--r--   0        0        0      251 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_disc.openbb
+-rw-r--r--   0        0        0      145 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_dps.openbb
+-rw-r--r--   0        0        0     1874 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb
+-rw-r--r--   0        0        0       44 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_base.openbb
+-rw-r--r--   0        0        0       31 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_epsfc.openbb
+-rw-r--r--   0        0        0       31 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa_revfc.openbb
+-rw-r--r--   0        0        0      470 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_gov.openbb
+-rw-r--r--   0        0        0      276 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ins.openbb
+-rw-r--r--   0        0        0      340 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options.openbb
+-rw-r--r--   0        0        0       91 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_payoff.openbb
+-rw-r--r--   0        0        0      121 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_pricing.openbb
+-rw-r--r--   0        0        0       82 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_options_screen.openbb
+-rw-r--r--   0        0        0      644 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb
+-rw-r--r--   0        0        0      170 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_scr.openbb
+-rw-r--r--   0        0        0      347 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_sia.openbb
+-rw-r--r--   0        0        0      717 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb
+-rw-r--r--   0        0        0       82 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_th.openbb
+-rw-r--r--   0        0        0       65 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/test_jupyter_base.openbb
+-rw-r--r--   0        0        0       16 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/test_keys_.openbb
+-rw-r--r--   0        0        0       46 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/test_news.openbb
+-rw-r--r--   0        0        0     1072 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/models/hub_credentials.json
+-rw-r--r--   0        0        0      380 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/models/local_credentials.json
+-rw-r--r--   0        0        0    17970 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
+-rw-r--r--   0        0        0    29757 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
+-rw-r--r--   0        0        0      310 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/routines/routine_example.openbb
+-rw-r--r--   0        0        0    22698 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/sources/openbb_default.json
+-rw-r--r--   0        0        0     2332 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
+-rw-r--r--   0        0        0     2354 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
+-rw-r--r--   0        0        0     2341 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
+-rw-r--r--   0        0        0     2316 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
+-rw-r--r--   0        0        0     2316 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
+-rw-r--r--   0        0        0     2346 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
+-rw-r--r--   0        0        0     2336 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
+-rw-r--r--   0        0        0     2346 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
+-rw-r--r--   0        0        0     2307 2023-04-11 00:09:08.344310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
+-rw-r--r--   0        0        0     2309 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
+-rw-r--r--   0        0        0     2329 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
+-rw-r--r--   0        0        0     2353 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
+-rw-r--r--   0        0        0     2360 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
+-rw-r--r--   0        0        0     2320 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
+-rw-r--r--   0        0        0     2344 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
+-rw-r--r--   0        0        0     2315 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
+-rw-r--r--   0        0        0     2346 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
+-rw-r--r--   0        0        0     2376 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
+-rw-r--r--   0        0        0     2326 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Health.ini
+-rw-r--r--   0        0        0     2307 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
+-rw-r--r--   0        0        0     2320 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
+-rw-r--r--   0        0        0     2324 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
+-rw-r--r--   0        0        0     2334 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
+-rw-r--r--   0        0        0     2324 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
+-rw-r--r--   0        0        0     2313 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
+-rw-r--r--   0        0        0     2341 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
+-rw-r--r--   0        0        0     2296 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
+-rw-r--r--   0        0        0     2367 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
+-rw-r--r--   0        0        0     2342 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
+-rw-r--r--   0        0        0     2361 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
+-rw-r--r--   0        0        0     2351 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
+-rw-r--r--   0        0        0     2336 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
+-rw-r--r--   0        0        0     2322 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
+-rw-r--r--   0        0        0     2310 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
+-rw-r--r--   0        0        0     2326 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
+-rw-r--r--   0        0        0     2341 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
+-rw-r--r--   0        0        0     2299 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
+-rw-r--r--   0        0        0     2316 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
+-rw-r--r--   0        0        0     2342 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
+-rw-r--r--   0        0        0     2381 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
+-rw-r--r--   0        0        0     2314 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
+-rw-r--r--   0        0        0    34473 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/template.ini
+-rw-r--r--   0        0        0    34519 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/whales.ini
+-rw-r--r--   0        0        0     2688 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/README.md
+-rw-r--r--   0        0        0     4195 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/high_iv.ini
+-rw-r--r--   0        0        0     4210 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini
+-rw-r--r--   0        0        0     3925 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini
+-rw-r--r--   0        0        0     4202 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini
+-rw-r--r--   0        0        0     4079 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/template.ini
+-rwxr-xr-x   0        0        0      282 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
+-rw-r--r--   0        0        0    21940 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
+-rwxr-xr-x   0        0        0      315 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
+-rwxr-xr-x   0        0        0      464 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
+-rw-r--r--   0        0        0      413 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
+-rwxr-xr-x   0        0        0      184 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
+-rwxr-xr-x   0        0        0      364 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
+-rw-r--r--   0        0        0      326 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
+-rw-r--r--   0        0        0      193 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
+-rw-r--r--   0        0        0      241 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
+-rwxr-xr-x   0        0        0      335 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
+-rw-r--r--   0        0        0      286 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
+-rwxr-xr-x   0        0        0      167 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
+-rw-r--r--   0        0        0      221 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
+-rwxr-xr-x   0        0        0      255 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
+-rwxr-xr-x   0        0        0      518 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
+-rw-r--r--   0        0        0      302 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
+-rwxr-xr-x   0        0        0      279 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
+-rw-r--r--   0        0        0      316 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
+-rw-r--r--   0        0        0      349 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
+-rwxr-xr-x   0        0        0      295 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
+-rwxr-xr-x   0        0        0      274 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
+-rwxr-xr-x   0        0        0      328 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
+-rwxr-xr-x   0        0        0      301 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
+-rwxr-xr-x   0        0        0      212 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
+-rwxr-xr-x   0        0        0      295 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
+-rw-r--r--   0        0        0      337 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
+-rw-r--r--   0        0        0      280 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
+-rw-r--r--   0        0        0      246 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
+-rw-r--r--   0        0        0      360 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
+-rwxr-xr-x   0        0        0      222 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
+-rwxr-xr-x   0        0        0      260 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
+-rwxr-xr-x   0        0        0      197 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
+-rwxr-xr-x   0        0        0      211 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
+-rwxr-xr-x   0        0        0      201 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
+-rwxr-xr-x   0        0        0      203 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
+-rwxr-xr-x   0        0        0      179 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
+-rwxr-xr-x   0        0        0      276 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
+-rwxr-xr-x   0        0        0      272 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
+-rwxr-xr-x   0        0        0      299 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
+-rwxr-xr-x   0        0        0      293 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
+-rwxr-xr-x   0        0        0      286 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
+-rw-r--r--   0        0        0      209 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
+-rwxr-xr-x   0        0        0      272 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
+-rwxr-xr-x   0        0        0      675 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
+-rwxr-xr-x   0        0        0      315 2023-04-11 00:09:08.348310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
+-rw-r--r--   0        0        0   358460 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
+-rw-r--r--   0        0        0      972 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
+-rw-r--r--   0        0        0     2086 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
+-rw-r--r--   0        0        0     2750 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0      203 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
+-rw-r--r--   0        0        0      970 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
+-rw-r--r--   0        0        0     2035 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.mplstyle
+-rw-r--r--   0        0        0    24077 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0      202 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
+-rw-r--r--   0        0        0     2607 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0      186 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
+-rw-r--r--   0        0        0      144 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/__init__.py
+-rw-r--r--   0        0        0    81373 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_fund_ID.csv
+-rw-r--r--   0        0        0      834 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_model.py
+-rw-r--r--   0        0        0     3941 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_view.py
+-rw-r--r--   0        0        0     6535 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mstarpy_model.py
+-rw-r--r--   0        0        0     7883 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mstarpy_view.py
+-rw-r--r--   0        0        0    15141 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mutual_fund_controller.py
+-rw-r--r--   0        0        0     6040 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mutual_funds_utils.py
+-rw-r--r--   0        0        0    51056 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/parent_classes.py
+-rw-r--r--   0        0        0       61 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/__init__.py
+-rw-r--r--   0        0        0    15080 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/allocation_model.py
+-rw-r--r--   0        0        0    12944 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/attribution_model.py
+-rw-r--r--   0        0        0      417 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/__init__.py
+-rw-r--r--   0        0        0     3214 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/bro_controller.py
+-rw-r--r--   0        0        0     1121 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/brokers_helpers.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/__init__.py
+-rw-r--r--   0        0        0     8211 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
+-rw-r--r--   0        0        0     9561 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
+-rw-r--r--   0        0        0     4495 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
+-rw-r--r--   0        0        0     4666 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/__init__.py
+-rw-r--r--   0        0        0    12789 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
+-rw-r--r--   0        0        0    15571 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
+-rw-r--r--   0        0        0    15670 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
+-rw-r--r--   0        0        0     3894 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
+-rw-r--r--   0        0        0     3002 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
+-rw-r--r--   0        0        0     2482 2023-04-11 00:09:08.352310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
+-rw-r--r--   0        0        0    30861 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/metrics_model.py
+-rw-r--r--   0        0        0    54979 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_controller.py
+-rw-r--r--   0        0        0    39188 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_engine.py
+-rw-r--r--   0        0        0     9643 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_helper.py
+-rw-r--r--   0        0        0    60205 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_model.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/__init__.py
+-rw-r--r--   0        0        0     5255 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
+-rw-r--r--   0        0        0     2106 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
+-rw-r--r--   0        0        0   120571 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
+-rw-r--r--   0        0        0   155050 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
+-rw-r--r--   0        0        0     2773 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
+-rw-r--r--   0        0        0    13116 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
+-rw-r--r--   0        0        0     5965 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
+-rw-r--r--   0        0        0     5346 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
+-rw-r--r--   0        0        0     4427 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
+-rw-r--r--   0        0        0   138034 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
+-rw-r--r--   0        0        0     8587 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
+-rw-r--r--   0        0        0   103568 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_model.py
+-rw-r--r--   0        0        0    24186 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_view.py
+-rw-r--r--   0        0        0    11390 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/statics.py
+-rw-r--r--   0        0        0    12009 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
+-rw-r--r--   0        0        0    54944 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_view.py
+-rw-r--r--   0        0        0     8433 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/statics.py
+-rw-r--r--   0        0        0     2877 2023-04-11 00:09:08.356310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reporting.md
+-rw-r--r--   0        0        0  1028287 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
+-rw-r--r--   0        0        0     2839 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/__init__.py
+-rw-r--r--   0        0        0      443 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/data/crypto_tickers.csv
+-rw-r--r--   0        0        0      437 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/data/etf_tickers.csv
+-rw-r--r--   0        0        0      222 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/data/stocks_tickers.csv
+-rw-r--r--   0        0        0     9716 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/reports_controller.py
+-rw-r--r--   0        0        0    12310 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/reports_model.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.360310 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/stored/.gitkeep
+-rw-r--r--   0        0        0  1076317 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
+-rw-r--r--   0        0        0     5214 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/OpenBB_reports_logo.png
+-rw-r--r--   0        0        0    32298 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/crypto.ipynb
+-rw-r--r--   0        0        0    23012 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/economy.ipynb
+-rw-r--r--   0        0        0    39776 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/equity.ipynb
+-rw-r--r--   0        0        0     9851 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/etf.ipynb
+-rw-r--r--   0        0        0     2782 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/floppy-disc.png
+-rw-r--r--   0        0        0     8557 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/forecast.ipynb
+-rw-r--r--   0        0        0    17654 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/forex.ipynb
+-rw-r--r--   0        0        0    14912 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/portfolio.ipynb
+-rw-r--r--   0        0        0    11247 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widget_helpers.py
+-rw-r--r--   0        0        0      205 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/card.j2
+-rw-r--r--   0        0        0     3556 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/report.css
+-rw-r--r--   0        0        0      474 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/report.j2
+-rw-r--r--   0        0        0      119 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/row.j2
+-rw-r--r--   0        0        0      896 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/style.css
+-rw-r--r--   0        0        0     9967 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/rich_config.py
+-rw-r--r--   0        0        0    30901 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/sdk.py
+-rw-r--r--   0        0        0    28198 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/settings_controller.py
+-rw-r--r--   0        0        0     7105 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/sources_controller.py
+-rw-r--r--   0        0        0      357 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.368311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/__init__.py
+-rw-r--r--   0        0        0    10448 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_controller.py
+-rw-r--r--   0        0        0     8126 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_model.py
+-rw-r--r--   0        0        0     9046 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0    29872 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
+-rw-r--r--   0        0        0     3541 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3761 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     1931 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/cboe_model.py
+-rw-r--r--   0        0        0      969 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/cboe_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/__init__.py
+-rw-r--r--   0        0        0    37655 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/ca_controller.py
+-rw-r--r--   0        0        0     4871 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     5785 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1328 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     2679 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
+-rw-r--r--   0        0        0     1539 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
+-rw-r--r--   0        0        0    12381 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     5757 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     1690 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/polygon_model.py
+-rw-r--r--   0        0        0     1379 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0     8073 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    10157 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/__init__.py
+-rw-r--r--   0        0        0    20377 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
+-rw-r--r--   0        0        0    10009 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
+-rw-r--r--   0        0        0     7203 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
+-rw-r--r--   0        0        0     1093 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
+-rw-r--r--   0        0        0     1200 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
+-rw-r--r--   0        0        0     1387 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
+-rw-r--r--   0        0        0     4648 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
+-rw-r--r--   0        0        0     6836 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
+-rw-r--r--   0        0        0     3470 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
+-rw-r--r--   0        0        0     1882 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
+-rw-r--r--   0        0        0     1385 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
+-rw-r--r--   0        0        0     5053 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
+-rw-r--r--   0        0        0     9997 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
+-rw-r--r--   0        0        0     1166 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
+-rw-r--r--   0        0        0     3613 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
+-rw-r--r--   0        0        0      668 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
+-rw-r--r--   0        0        0     1271 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
+-rw-r--r--   0        0        0     5740 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/databento_model.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/__init__.py
+-rw-r--r--   0        0        0     4169 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/ark_model.py
+-rw-r--r--   0        0        0     2589 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/ark_view.py
+-rw-r--r--   0        0        0    31510 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/disc_controller.py
+-rw-r--r--   0        0        0      483 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/disc_helpers.py
+-rw-r--r--   0        0        0     2696 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fidelity_model.py
+-rw-r--r--   0        0        0     2680 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fidelity_view.py
+-rw-r--r--   0        0        0     4164 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finnhub_model.py
+-rw-r--r--   0        0        0     2510 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finnhub_view.py
+-rw-r--r--   0        0        0     1731 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finviz_model.py
+-rw-r--r--   0        0        0     3084 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finviz_view.py
+-rw-r--r--   0        0        0     2562 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fmp_view.py
+-rw-r--r--   0        0        0     3051 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/nasdaq_model.py
+-rw-r--r--   0        0        0     3406 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/nasdaq_view.py
+-rw-r--r--   0        0        0     7080 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/seeking_alpha_model.py
+-rw-r--r--   0        0        0     4803 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/seeking_alpha_view.py
+-rw-r--r--   0        0        0     1120 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/shortinterest_model.py
+-rw-r--r--   0        0        0     2566 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/shortinterest_view.py
+-rw-r--r--   0        0        0     4113 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/yahoofinance_model.py
+-rw-r--r--   0        0        0     5871 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/yahoofinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/__init__.py
+-rw-r--r--   0        0        0    24082 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/av_model.py
+-rw-r--r--   0        0        0    14910 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/av_view.py
+-rw-r--r--   0        0        0    10834 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
+-rw-r--r--   0        0        0     7680 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
+-rw-r--r--   0        0        0     1833 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
+-rw-r--r--   0        0        0     2347 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
+-rw-r--r--   0        0        0    14888 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
+-rw-r--r--   0        0        0     4279 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
+-rw-r--r--   0        0        0    44464 2023-04-11 00:09:08.372311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
+-rw-r--r--   0        0        0     1925 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
+-rw-r--r--   0        0        0     1205 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
+-rw-r--r--   0        0        0     2396 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
+-rw-r--r--   0        0        0     4904 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
+-rw-r--r--   0        0        0    81233 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
+-rw-r--r--   0        0        0      266 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
+-rw-r--r--   0        0        0     1389 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3518 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3419 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
+-rw-r--r--   0        0        0     2484 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
+-rw-r--r--   0        0        0    22210 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
+-rw-r--r--   0        0        0    25688 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
+-rw-r--r--   0        0        0     6417 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
+-rw-r--r--   0        0        0    11855 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py
+-rw-r--r--   0        0        0     1509 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py
+-rw-r--r--   0        0        0     2217 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     1259 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     5391 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
+-rw-r--r--   0        0        0     4361 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
+-rw-r--r--   0        0        0     7593 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0    11162 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
+-rw-r--r--   0        0        0     2059 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
+-rw-r--r--   0        0        0    11829 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    14679 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/__init__.py
+-rw-r--r--   0        0        0    18461 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/gov_controller.py
+-rw-r--r--   0        0        0    15719 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/quiverquant_model.py
+-rw-r--r--   0        0        0    21407 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/quiverquant_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/__init__.py
+-rw-r--r--   0        0        0     2062 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/businessinsider_model.py
+-rw-r--r--   0        0        0     5102 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/businessinsider_view.py
+-rw-r--r--   0        0        0     1125 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/finviz_model.py
+-rw-r--r--   0        0        0     1171 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/finviz_view.py
+-rw-r--r--   0        0        0    32744 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/insider_controller.py
+-rw-r--r--   0        0        0    87496 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/openinsider_model.py
+-rw-r--r--   0        0        0     7695 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/openinsider_view.py
+-rw-r--r--   0        0        0     4909 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/sdk_helper.py
+-rw-r--r--   0        0        0    76085 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/mappings/Mic_Codes.csv
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/__init__.py
+-rw-r--r--   0        0        0     1757 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/alphaquery_model.py
+-rw-r--r--   0        0        0     1713 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/alphaquery_view.py
+-rw-r--r--   0        0        0     1161 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/barchart_model.py
+-rw-r--r--   0        0        0     1137 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/barchart_view.py
+-rw-r--r--   0        0        0     1526 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/calculator_model.py
+-rw-r--r--   0        0        0     2416 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/calculator_view.py
+-rw-r--r--   0        0        0     2777 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/chartexchange_model.py
+-rw-r--r--   0        0        0     3211 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/chartexchange_view.py
+-rw-r--r--   0        0        0     2433 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/fdscanner_model.py
+-rw-r--r--   0        0        0     1672 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/fdscanner_view.py
+-rw-r--r--   0        0        0    21092 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_controller.py
+-rw-r--r--   0        0        0     9884 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_model.py
+-rw-r--r--   0        0        0     3968 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_view.py
+-rw-r--r--   0        0        0    10030 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/intrinio_model.py
+-rw-r--r--   0        0        0     6101 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/intrinio_view.py
+-rw-r--r--   0        0        0     7097 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/nasdaq_model.py
+-rw-r--r--   0        0        0    22486 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/op_helpers.py
+-rw-r--r--   0        0        0    51898 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_controller.py
+-rw-r--r--   0        0        0    10556 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_sdk_helper.py
+-rw-r--r--   0        0        0    14169 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.376311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/__init__.py
+-rw-r--r--   0        0        0     5686 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/screener_controller.py
+-rw-r--r--   0        0        0     9556 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/syncretism_model.py
+-rw-r--r--   0        0        0     5566 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/syncretism_view.py
+-rw-r--r--   0        0        0     8295 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/tradier_model.py
+-rw-r--r--   0        0        0     2561 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/tradier_view.py
+-rw-r--r--   0        0        0     7674 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/yfinance_model.py
+-rw-r--r--   0        0        0    11615 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0     2260 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/beta_model.py
+-rw-r--r--   0        0        0     2798 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/beta_view.py
+-rw-r--r--   0        0        0     3187 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/factors_model.py
+-rw-r--r--   0        0        0      687 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/factors_view.py
+-rw-r--r--   0        0        0    38741 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0      447 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/research/__init__.py
+-rw-r--r--   0        0        0     6218 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/research/res_controller.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/__init__.py
+-rw-r--r--   0        0        0    46491 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/finviz_model.py
+-rw-r--r--   0        0        0     6981 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/finviz_view.py
+-rw-r--r--   0        0        0    21493 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_controller.py
+-rw-r--r--   0        0        0      944 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_helper.py
+-rw-r--r--   0        0        0     2562 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_view.py
+-rw-r--r--   0        0        0    27077 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stock_statics.py
+-rw-r--r--   0        0        0    27315 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_controller.py
+-rw-r--r--   0        0        0    33068 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_helper.py
+-rw-r--r--   0        0        0    10576 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_model.py
+-rw-r--r--   0        0        0     1241 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finbrain_model.py
+-rw-r--r--   0        0        0      644 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finbrain_view.py
+-rw-r--r--   0        0        0      761 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finviz_model.py
+-rw-r--r--   0        0        0     1229 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finviz_view.py
+-rw-r--r--   0        0        0     1532 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/rsp_model.py
+-rw-r--r--   0        0        0     2386 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/rsp_view.py
+-rw-r--r--   0        0        0    63334 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     3260 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/tradingview_model.py
+-rw-r--r--   0        0        0     1985 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/tradingview_view.py
+-rw-r--r--   0        0        0      334 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/__init__.py
+-rw-r--r--   0        0        0     5328 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/bursa_model.py
+-rw-r--r--   0        0        0     2202 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/bursa_view.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/data/__init__.py
+-rw-r--r--   0        0        0    28098 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
+-rw-r--r--   0        0        0     1466 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
+-rw-r--r--   0        0        0     1378 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
+-rw-r--r--   0        0        0    10137 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
+-rw-r--r--   0        0        0      614 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
+-rw-r--r--   0        0        0    42825 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/terminal_controller.py
+-rw-r--r--   0        0        0    14336 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/terminal_helper.py
+-rw-r--r--   0        0        0     3848 2023-04-11 00:09:08.380311 openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/thought_of_the_day.py
+-rw-r--r--   0        0        0     5811 2023-04-11 00:09:10.080348 openbb_nightly-3.0.0rc1.dev20230411/pyproject.toml
+-rw-r--r--   0        0        0      945 2023-04-11 00:09:08.384311 openbb_nightly-3.0.0rc1.dev20230411/terminal.py
+-rw-r--r--   0        0        0     2293 2023-04-11 00:09:10.084348 openbb_nightly-3.0.0rc1.dev20230411/website/pypi.md
+-rw-r--r--   0        0        0     7850 1970-01-01 00:00:00.000000 openbb_nightly-3.0.0rc1.dev20230411/PKG-INFO
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/LICENSE` & `openbb_nightly-3.0.0rc1.dev20230411/LICENSE`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/SDK_README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/SDK_README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/account/account_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/account/account_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/alt_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/alt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/countries.txt` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/countries.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/covid/covid_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/covid/covid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/hackernews_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/hackernews_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/hackernews_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/hackernews_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/github_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/github_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/github_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/github_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/oss_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/oss_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/runa_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/runa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/oss/runa_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/oss/runa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/landRegistry_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/landRegistry_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/landRegistry_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/landRegistry_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/alternative/realestate/realestate_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/alternative/realestate/realestate_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/base_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/base_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/google_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/google_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/google_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/google_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/reddit_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/reddit_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/stocktwits_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/stocktwits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/stocktwits_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/stocktwits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/twitter_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/twitter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/behavioural_analysis/twitter_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/behavioural_analysis/twitter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/common_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/common_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/feedparser_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/feedparser_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/feedparser_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/feedparser_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/newsapi_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/newsapi_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/newsapi_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/newsapi_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/qa_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/qa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/qa_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/qa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/rolling_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/rolling_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/quantitative_analysis/rolling_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/quantitative_analysis/rolling_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/custom_indicators_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/custom_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/custom_indicators_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/custom_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/momentum_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/momentum_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/momentum_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/momentum_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/overlap_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/overlap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/overlap_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/overlap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/ta_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/trend_indicators_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/trend_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/trend_indicators_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/trend_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volatility_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volatility_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volatility_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volatility_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volume_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volume_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/technical_analysis/volume_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/technical_analysis/volume_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/ultima_newsmonitor_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/ultima_newsmonitor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/common/ultima_newsmonitor_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/common/ultima_newsmonitor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/config_terminal.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/config_terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/completer/choices.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/completer/choices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/config/paths.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/config/paths.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/config/paths_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/config/paths_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/integration_tests/README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/integration_tests/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/integration_tests/integration_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/integration_tests/integration_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/log_sender.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/log_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/logging_clock.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/logging_clock.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/collection/s3_sender.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/collection/s3_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/common.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/common.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/custom_logger.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/custom_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/directories.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/directories.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/expired_files.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/formatter_with_exceptions.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/path_tracking_file_handler.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/settings.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/log/generation/settings_logger.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/log/generation/settings_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/__init__.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/base_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/credentials_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/credentials_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/preferences_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/preferences_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/profile_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/profile_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/sources_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/sources_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/system_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/system_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/models/user_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/models/user_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/assets/Terminal_icon.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/assets/icon.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/assets/icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/backend.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/config/openbb_styles.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/no_import.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/no_import.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/old_table.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/old_table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,31 +83,32 @@
             The name of the Rich style to use, by default ""
         """
         self.plt_style = plt_style or self.plt_style
         self.load_available_styles()
         self.load_style(plt_style)
         self.apply_console_style(console_style)
 
-    def apply_console_style(self, style: Optional[str] = "") -> None:
+    def apply_console_style(self, style: Optional[str] = None) -> None:
         """Apply the style to the console."""
 
-        if style in self.console_styles_available:
-            json_path: Optional[Path] = self.console_styles_available[style]
-        else:
-            self.load_available_styles()
+        if style:
             if style in self.console_styles_available:
-                json_path = self.console_styles_available[style]
+                json_path: Optional[Path] = self.console_styles_available[style]
             else:
-                console.print("\nInvalid console style. Using default.")
-                json_path = self.console_styles_available.get("dark", None)
+                self.load_available_styles()
+                if style in self.console_styles_available:
+                    json_path = self.console_styles_available[style]
+                else:
+                    console.print(f"\nInvalid console style '{style}', using default.")
+                    json_path = self.console_styles_available.get("dark", None)
 
-        if json_path:
-            self.console_style = self.load_json_style(json_path)
-        else:
-            console.print("Error loading default.")
+            if json_path:
+                self.console_style = self.load_json_style(json_path)
+            else:
+                console.print("Error loading default.")
 
     def apply_style(self, style: Optional[str] = "") -> None:
         """Apply the style to the libraries."""
         if not style:
             style = get_current_user().preferences.THEME
 
         if style != self.plt_style:
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/base.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/data_classes.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/plotly_ta/ta_class.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/table.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/bar_menus.js` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/bar_menus.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/fonts/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/fonts/FiraCode-VF.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/css/style.css` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/css/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -221,16 +221,17 @@
   margin-right: 10px;
   background: #0f0f0f !important;
   border: 1px solid #404040;
   box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.06);
   border-radius: 8px;
 }
 
+
 .modebar-group:nth-of-type(1):after {
-  content: "Chart Tools";
+  content: "Panning Tools";
   height: fit-content;
   width: fit-content;
   position: absolute;
   display: none;
 }
 
 .modebar-group:nth-of-type(1):hover:after {
@@ -245,15 +246,15 @@
   border-radius: 8px;
   top: -40px;
   left: 50%;
   transform: translateX(-50%);
 }
 
 .modebar-group:nth-of-type(2):after {
-  content: "Panning Tools";
+  content: "Indicator Tools";
   height: fit-content;
   width: fit-content;
   position: absolute;
   display: none;
 }
 
 .modebar-group:nth-of-type(2):hover:after {
@@ -268,15 +269,15 @@
   border-radius: 8px;
   top: -40px;
   left: 50%;
   transform: translateX(-50%);
 }
 
 .modebar-group:nth-of-type(3):after {
-  content: "Drawing Tools";
+  content: "Chart Tools";
   height: fit-content;
   width: fit-content;
   position: absolute;
   display: none;
 }
 
 .modebar-group:nth-of-type(3):hover:after {
@@ -291,29 +292,52 @@
   border-radius: 8px;
   top: -40px;
   left: 50%;
   transform: translateX(-50%);
 }
 
 .modebar-group:nth-of-type(4):after {
-  content: "Export Tools";
+  content: "Drawing Tools";
   height: fit-content;
   width: fit-content;
   position: absolute;
   display: none;
 }
 
 .modebar-group:nth-of-type(4):hover:after {
   padding: 10px;
   display: block;
   font-size: 10px;
   color: white;
   cursor: pointer;
   background: #0f0f0f !important;
   border: 1px solid #404040;
+  box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.06);
+  border-radius: 8px;
+  top: -40px;
+  left: 50%;
+  transform: translateX(-50%);
+}
+
+.modebar-group:nth-of-type(5):after {
+  content: "Export Tools";
+  height: fit-content;
+  width: fit-content;
+  position: absolute;
+  display: none;
+}
+
+.modebar-group:nth-of-type(5):hover:after {
+  padding: 10px;
+  display: block;
+  font-size: 10px;
+  color: white;
+  cursor: pointer;
+  background: #0f0f0f !important;
+  border: 1px solid #404040;
   box-shadow: 0px 4px 24px rgba(0, 0, 0, 0.06);
   border-radius: 8px;
   top: -40px;
   left: 50%;
   transform: translateX(-50%);
 }
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/helpers.js` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/helpers.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -369,15 +369,16 @@
     // changes the style of the button when it is pressed
     // title is the title of the button
     // active is true if the button is active, false otherwise
 
     let button = globals.barButtons[title];
 
     if (!active) {
-        button.style.border = "1px solid rgba(255, 0, 0, 0.7)";
+        button.style.border = "1px solid rgba(0, 151, 222, 1.0)";
         button.style.borderRadius = "5px";
-        button.style.boxShadow = "0 0 5px rgba(255, 0, 0, 0.7)";
+        button.style.borderpadding = "5px";
+        button.style.boxShadow = "0 0 5px rgba(0, 151, 222, 1.0)";
     } else {
         button.style.border = "transparent";
         button.style.boxShadow = "none";
     }
 }
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/main.js` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/main.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -73,50 +73,49 @@
         scrollZoom: true,
         responsive: true,
         displaylogo: false,
         displayModeBar: true,
         modeBarButtonsToRemove: ["lasso2d", "select2d", "downloadImage"],
         modeBarButtons: [
             [{
-                    name: "Download CSV (Ctrl+S)",
+                    name: "Download CSV (Ctrl+Shift+S)",
                     icon: ICONS.downloadCsv,
                     click: function(gd) {
                         loadingOverlay("Saving CSV");
                         setTimeout(function() {
                             downloadData(gd);
                         }, 500);
                         setTimeout(function() {
                             loading.classList.remove("show");
                         }, 1000);
                     },
-                },
-                // {
-                //   name: "Upload Image (Ctrl+U)",
-                //   icon: Plotly.Icons.uploadImage,
-                //   click: function (gd) {
-                //     downloadImage();
-                //   },
-                // },
-                {
-                    name: "Save Chart as Image",
+                }, {
+                    name: "Download PNG (Ctrl+S)",
                     icon: ICONS.downloadImage,
                     click: function() {
-                        loadingOverlay("Saving Image");
+                        loadingOverlay("Saving PNG");
                         hideModebar();
                         non_blocking(function() {
                             downloadImage(globals.filename, "png");
                             setTimeout(function() {
                                 setTimeout(function() {
                                     loading.classList.remove("show");
                                     hideModebar();
                                 }, 50);
                             }, 25);
                         }, 2)();
                     },
                 },
+                // {
+                //   name: "Upload Image (Ctrl+U)",
+                //   icon: Plotly.Icons.uploadImage,
+                //   click: function (gd) {
+                //     downloadImage();
+                //   },
+                // },
             ],
             [{
                     name: "Edit Color (Ctrl+E)",
                     icon: ICONS.changeColor,
                     click: function() {
                         // We need to check if the button is active or not
                         let title = "Edit Color (Ctrl+E)";
@@ -132,37 +131,42 @@
                 },
                 "drawline",
                 "drawopenpath",
                 "drawcircle",
                 "drawrect",
                 "eraseshape",
             ],
-            ["zoomIn2d", "zoomOut2d", "autoScale2d", "zoom2d", "pan2d"],
             [{
-                    name: "Add Text (Ctrl+T)",
-                    icon: ICONS.addText,
-                    click: function() {
-                        openPopup("popup_text");
-                    },
-                }, {
-                    name: "Change Titles (Ctrl+Shift+T)",
-                    icon: ICONS.changeTitle,
-                    click: function() {
-                        openPopup("popup_title");
-                    },
-                }, {
-                    name: "Plot CSV (Ctrl+Shift+C)",
-                    icon: ICONS.plotCsv,
-                    click: function() {
-                        // We make sure to close any other popup that might be open
-                        // before opening the CSV popup
-                        closePopup();
-                        openPopup("popup_csv");
-                    },
-                }, {
+                name: "Overlay chart from CSV (Ctrl+O)",
+                icon: ICONS.plotCsv,
+                click: function() {
+                    // We make sure to close any other popup that might be open
+                    // before opening the CSV popup
+                    closePopup();
+                    openPopup("popup_csv");
+                },
+            }, {
+                name: "Add Text (Ctrl+T)",
+                icon: ICONS.addText,
+                click: function() {
+                    openPopup("popup_text");
+                },
+            }, {
+                name: "Change Titles (Ctrl+Shift+T)",
+                icon: ICONS.changeTitle,
+                click: function() {
+                    openPopup("popup_title");
+                },
+            }, ],
+            [
+                "hoverClosestCartesian",
+                "hoverCompareCartesian",
+                "toggleSpikelines",
+            ],
+            [{
                     name: "Auto Scale (Ctrl+Shift+A)",
                     icon: Plotly.Icons.autoscale,
                     click: function() {
                         // We need to check if the button is active or not
                         let title = "Auto Scale (Ctrl+Shift+A)";
                         let button = globals.barButtons[title];
                         let active = true;
@@ -181,17 +185,19 @@
                             // If the button isn't active, we remove the listener so
                             // the graphs don't autoscale anymore
                             globals.CHART_DIV.removeAllListeners("plotly_relayout");
                         }
                         button_pressed(title, active);
                     },
                 },
-                "hoverClosestCartesian",
-                "hoverCompareCartesian",
-                "toggleSpikelines",
+                "zoomIn2d",
+                "zoomOut2d",
+                "autoScale2d",
+                "zoom2d",
+                "pan2d",
             ],
         ],
     };
     graphs.layout.title = "";
 
     // We make sure to fill in any missing layout properties with default values
     if (!("font" in graphs.layout)) {
@@ -210,14 +216,17 @@
             r: 0,
             b: 0,
             t: 0,
             pad: 2,
         };
     }
 
+    // RIP: Juan hated it so had to remove it
+    // graphs.layout.xaxis.tickangle = -20;
+
     graphs.layout.autosize = true;
     // We set the height and width to undefined, so that plotly.js can
     // automatically resize the chart to fit the PyWry window
     delete graphs.layout.height;
     delete graphs.layout.width;
 
     if (graphs.layout.annotations != undefined) {
@@ -348,31 +357,31 @@
 
     // We setup keyboard shortcuts custom to OpenBB
     window.document.addEventListener("keydown", function(e) {
         if (e.key.toLowerCase() == "h" && (e.ctrlKey || e.metaKey)) {
             e.preventDefault();
             hideModebar();
         }
-        if (e.ctrlKey && e.key.toLowerCase() == "t") {
-            openPopup("popup_text");
-        }
-        if (e.ctrlKey && e.key.toLowerCase() == "e") {
-            changeColor();
-        }
-        if (e.ctrlKey && e.shiftKey && e.key.toLowerCase() == "t") {
-            openPopup("popup_title");
-        }
-        if (e.ctrlKey && e.key.toLowerCase() == "s") {
-            downloadData(globals.CHART_DIV);
-        }
-        if (e.ctrlKey && e.shiftKey && e.key.toLowerCase() == "c") {
-            e.preventDefault();
-            openPopup("popup_csv");
-        }
-        if (e.key == "Escape") {
+
+        if (e.ctrlKey) {
+            if (e.shiftKey && e.key.toLowerCase() == "t") {
+                openPopup("popup_title");
+            } else if (e.key.toLowerCase() == "t") {
+                openPopup("popup_text");
+            } else if (e.key.toLowerCase() == "e") {
+                changeColor();
+            } else if (e.shiftKey && e.key.toLowerCase() == "s") {
+                downloadData(globals.CHART_DIV);
+            } else if (e.key.toLowerCase() == "s") {
+                downloadImage(globals.filename, "png");
+            } else if (e.key.toLowerCase() == "o") {
+                e.preventDefault();
+                openPopup("popup_csv");
+            }
+        } else if (e.key == "Escape") {
             closePopup();
         }
     });
 
     // send a relayout event to trigger the initial zoom/bars-resize
     // check if the xaxis.range is defined
     if (
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/main_table.js` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/main_table.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/plots/web/popups.js` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/plots/web/popups.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/scripts/sdk_audit.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/scripts/sdk_audit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/__init__.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/alt_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/alt_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/crypto_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/crypto_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/econometrics_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/econometrics_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/economy_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/economy_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/etf_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/etf_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/forecast_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/forecast_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/forex_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/forex_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/funds_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/funds_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/futures_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/futures_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/keys_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/keys_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/portfolio_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/portfolio_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/qa_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/qa_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/stocks_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/stocks_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/models/ta_sdk_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/models/ta_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/sdk_init.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/sdk_init.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map_forecasting.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map_forecasting.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trail_map_optimization.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trail_map_optimization.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sdk/trailmap.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sdk/trailmap.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/banner.txt` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/banner.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/current_system.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/current_system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/current_user.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/current_user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/env_handler.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/env_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/hub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/hub_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -675,15 +675,17 @@
     url = f"{base_url}sdk/token"
 
     headers = {"Authorization": auth_header}
 
     try:
         response = requests.get(url=url, headers=headers, timeout=timeout)
 
-        if response.status_code != 200:
+        if response.status_code == 404:
+            console.print("[red]No personal access token found.[/red]")
+        elif response.status_code != 200:
             console.print("[red]Failed to get personal access token.[/red]")
 
         return response
 
     except requests.exceptions.ConnectionError:
         console.print(f"\n{CONNECTION_ERROR_MSG}")
         return None
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/local_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/local_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/sdk_session.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/sdk_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/session_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/session_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/session_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/session_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/sources_handler.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/sources_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/session/utils.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/core/sources/utils.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/core/sources/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/coinbase_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/coinbase_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/coinpaprika_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/coinpaprika_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
             "Uses CoinGecko to grab coin data (price and market cap).",
         )
         parser.add_argument(
             "--vs",
             help="Coin to compare with",
             dest="vs",
             type=str,
-            # required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
             default=None,
         )
         parser.add_argument(
             "-p",
             "--price",
             help="Desired price",
             dest="price",
@@ -183,19 +183,17 @@
             dest="top",
             type=int,
             default=None,
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "--vs")
 
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
-        )
-
-        if ns_parser:
+        ):
             if self.symbol:
                 num_args = 0
                 for arg in vars(ns_parser):
                     if getattr(ns_parser, arg):
                         num_args = num_args + 1
                         if num_args > 1:
                             console.print("[red]Please chose only one flag[/red]\n")
@@ -236,27 +234,25 @@
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="price",
             description="""Display price and interval of confidence in real-time. [Source: Pyth]""",
         )
         parser.add_argument(
             "-s",
             "--symbol",
-            required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
             type=str,
             dest="symbol",
             help="Symbol of coin to load data for, ~100 symbols are available",
             choices=pyth_model.ASSETS.keys(),
             metavar="SYMBOL",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-s")
 
-        ns_parser = self.parse_known_args_and_warn(parser, other_args)
-
-        if ns_parser:
+        if ns_parser := self.parse_known_args_and_warn(parser, other_args):
             upper_symbol = ns_parser.symbol.upper()
             if "-USD" not in ns_parser.symbol:
                 upper_symbol += "-USD"
             if upper_symbol in pyth_model.ASSETS:
                 console.print(
                     "[param]If it takes too long, you can use 'Ctrl + C' to cancel.\n[/param]"
                 )
@@ -279,18 +275,17 @@
             "--log",
             help="Plot with y axis on log scale",
             action="store_true",
             default=False,
             dest="logy",
         )
 
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_BOTH_RAW_DATA_AND_FIGURES
-        )
-        if ns_parser:
+        ):
             if not self.symbol:
                 console.print("No coin loaded. First use `load {symbol}`\n")
                 return
             figure = plot_chart(
                 exchange=self.exchange,
                 source=self.source,
                 to_symbol=self.symbol,
@@ -381,19 +376,17 @@
             type=str,
             dest="coin",
             help="Symbol of coin to load data for, ~100 symbols are available",
             choices=finbrain_crypto_view.COINS,
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-c")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_BOTH_RAW_DATA_AND_FIGURES
-        )
-
-        if ns_parser:
+        ):
             finbrain_crypto_view.display_crypto_sentiment_analysis(
                 symbol=ns_parser.coin, export=ns_parser.export
             )
 
     @log_start_end(log=logger)
     def call_dd(self, _):
         """Process dd command"""
@@ -470,15 +463,15 @@
             """,
         )
         parser.add_argument(
             "-c",
             "--coin",
             help="Symbol Name or Id of Coin",
             dest="coin",
-            required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
             type=str,
         )
         parser.add_argument(
             "-k",
             "--key",
             dest="key",
             help="Specify by which column you would like to search: symbol, name, id",
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_models.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/crypto_views.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/crypto_views.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/binance_gecko_map.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/binance_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coingecko_categories.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coingecko_categories.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coingecko_coins.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coingecko_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/defillama_dapps.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/defillama_dapps.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/erc20_coins.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/erc20_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/finbrain_coins.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/finbrain_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/santiment_slugs.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/santiment_slugs.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/dataframe_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/dataframe_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/coindix_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/coindix_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/coindix_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/coindix_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/defi_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/defi_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/graph_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/graph_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/graph_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/graph_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/llama_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/llama_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/llama_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/llama_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/smartstake_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/smartstake_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/smartstake_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/smartstake_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/substack_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/substack_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/substack_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/substack_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terraengineer_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terraengineer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terraengineer_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terraengineer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/dappradar_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/dappradar_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/dappradar_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/dappradar_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/discovery_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/binance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/binance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/binance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/binance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/messari_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/messari_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/messari_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/messari_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nft_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nft_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/opensea_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/opensea_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/nft/opensea_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/nft/opensea_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/bitquery_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/bitquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/bitquery_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/bitquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/blockchain_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/blockchain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/blockchain_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/blockchain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/onchain_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/onchain_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/shroom_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/shroom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/shroom_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/shroom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/glassnode_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/glassnode_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/loanscan_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/loanscan_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/loanscan_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/loanscan_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/overview_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/overview_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/rekt_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/rekt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/rekt_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/rekt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pycoingecko_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pycoingecko_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pyth_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pyth_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/pyth_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/pyth_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/cryptocurrency/tools/tools_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/cryptocurrency/tools/tools_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_prompt_toolkit.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_prompt_toolkit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/coin_highs.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/coin_highs.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_crash.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_crash.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_supply.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_supply.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/luna_terra.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/luna_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/tvl.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/tvl.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/custom_reports/lunar_crash/ust_terra.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/custom_reports/lunar_crash/ust_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/dashboards_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/dashboards_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/stream/Forecasting.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/stream/Forecasting.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/stream/pages/Indicators.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/stream/pages/Indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/chains.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/chains.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/correlation.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/correlation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/futures.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/futures.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/shortdata.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/shortdata.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/dashboards/voila/stocks.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/dashboards/voila/stocks.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/decorators.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/econometrics_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/econometrics_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/regression_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/regression_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/econometrics/regression_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/econometrics/regression_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/alphavantage_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/alphavantage_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/alphavantage_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/alphavantage_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/commodity_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/commodity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/commodity_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/commodity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/cpi.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/datasets/harmonized_cpi.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/datasets/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/econdb_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/econdb_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/economy_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/economy_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/economy_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/economy_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/fred_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/fred_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/nasdaq_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/oecd_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/oecd_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/plot_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/plot_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/wsj_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/wsj_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/economy/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/economy/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/wsj_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/discovery/wsj_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/discovery/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/etf_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/etf_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/etfs.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/etfs.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/financedatabase_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/financedatabase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/financedatabase_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/financedatabase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/fmp_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/stockanalysis_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/stockanalysis_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/stockanalysis_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/stockanalysis_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/etf/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/etf/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/featflags_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/featflags_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/commercial_paper.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/corporate_spot_rates.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ecb_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ecb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ecb_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ecb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/econdb_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/econdb_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fixedincome_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fixedincome_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fred_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/fred_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/fred_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1082,30 +1082,30 @@
     fig = OpenBBFigure(yaxis_title="Yield (%)")
     fig.set_title(title)
 
     fig.add_scatter(x=df.index, y=df[series_id], name="Yield")
 
     if raw:
         # was a -iloc so we need to flip the index as we use head
-        df = pd.DataFrame(df, columns=[parameter])
+        df = pd.DataFrame(df, columns=[series_id])
         df = df.sort_index(ascending=False)
         print_rich_table(
             df,
             title=title,
             show_index=True,
             floatfmt=".3f",
             export=bool(export),
             limit=limit,
         )
 
     export_data(
         export,
         os.path.dirname(os.path.abspath(__file__)),
         series_id,
-        pd.DataFrame(df, columns=[parameter]) / 100,
+        pd.DataFrame(df, columns=[series_id]) / 100,
         sheet_name,
         fig,
     )
 
     return fig.show(external=external_axes)
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/ice_bofa_indices.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/oecd_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/oecd_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/fixedincome/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/fixedincome/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/anom_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/anom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/anom_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/anom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoarima_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoarima_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoarima_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoarima_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoces_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoces_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoces_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoces_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoets_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoets_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoets_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoets_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoselect_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoselect_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/autoselect_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/autoselect_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/brnn_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/brnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/brnn_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/brnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/expo_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/expo_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/expo_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/expo_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/forecast_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/forecast_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/linregr_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/linregr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/linregr_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/linregr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/mstl_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/mstl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/mstl_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/mstl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nbeats_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nbeats_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nbeats_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nbeats_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nhits_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nhits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/nhits_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/nhits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/regr_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/regr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/regr_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/regr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rnn_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rnn_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rwd_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rwd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/rwd_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/rwd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/seasonalnaive_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/seasonalnaive_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/seasonalnaive_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/seasonalnaive_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tcn_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tcn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tcn_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tcn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tft_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tft_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/tft_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/tft_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/theta_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/theta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/theta_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/theta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/trans_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/trans_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/trans_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/trans_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/whisper_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/whisper_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forecast/whisper_utils.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forecast/whisper_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/av_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/av_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/av_forex_currencies.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/av_forex_currencies.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/polygon_tickers.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/polygon_tickers.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/data/yahoofinance_forex.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/data/yahoofinance_forex.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/forex_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/forex_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/forex_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/forex_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/fxempire_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/fxempire_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/fxempire_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/fxempire_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/oanda/oanda_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/oanda/oanda_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/forex/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/forex/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/databento_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/databento_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/futures_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/futures_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/futures/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/futures/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helper_classes.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helper_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helper_funcs.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/helpers_denomination.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/helpers_denomination.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/intro.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/intro.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/keys_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/keys_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/loggers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/loggers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/menu.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/menu.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/futures/futures.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/futures/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/i18n/en.yml` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/i18n/en.yml`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/i18n/help_translation.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/i18n/help_translation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_dd.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_defi.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_onchain.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ov.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics_base.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_oanda.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po_show_plot_rpf.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio_po.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_bt.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_fa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/models/hub_credentials.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/models/hub_credentials.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/sources/openbb_default.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/sources/openbb_default.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Banks.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Banks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Construction.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Construction.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Health.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Health.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Legal.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Legal.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Mining.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Mining.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/template.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/insider/whales.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/insider/whales.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/high_iv.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/high_iv.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/iv_below_20day.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/liquid_otm.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/spy_30_delta.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/options/template.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/options/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/Consolas.ttf` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/Consolas.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.mplstyle` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.mplstyle` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_fund_ID.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_fund_ID.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/avanza_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/avanza_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mstarpy_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mstarpy_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mstarpy_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mstarpy_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mutual_fund_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mutual_fund_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/mutual_funds/mutual_funds_utils.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/mutual_funds/mutual_funds_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/parent_classes.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/parent_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1297,15 +1297,15 @@
         )
         parser.add_argument(
             "-c",
             "--coin",
             help="Coin to get. Must be coin symbol (e.g., btc, eth)",
             dest="coin",
             type=str,
-            required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
         )
 
         parser.add_argument(
             "-s",
             "--start",
             type=valid_date,
             default=(datetime.now() - timedelta(days=1100)).strftime("%Y-%m-%d"),
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/allocation_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/allocation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/attribution_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/attribution_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/bro_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/bro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/brokers_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/brokers_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/degiro/degiro_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/degiro/degiro_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/metrics_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/metrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_engine.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/excel_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/excel_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_engine.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/po_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/po_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/statics.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/portfolio_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/portfolio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/portfolio/statics.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/portfolio/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reporting.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reporting.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/README.md` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/reports_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/reports_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/reports_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/reports_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,16 +177,16 @@
 
     parameters_dict = {}
     for line in cell_lines:
         # Extract key and value from each line
         key, value = line.split("=")
         key = key.strip()
         value = value.strip()
-        # Add key-value pair to dictionary
-        parameters_dict[key] = value
+        # Add key-value pair to dictionary and remove quotes
+        parameters_dict[key] = value.replace('"', "")
 
     if "report_name" in parameters_dict:
         parameters_dict.pop("report_name")
 
     return parameters_dict
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/OpenBB_reports_logo.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/OpenBB_reports_logo.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/crypto.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/crypto.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/economy.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/economy.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944727620462446%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(7, 'futures_fig = OpenBBFigure.to_table(futures, "*

 * *            "print_index=True)')], delete: [17, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7]}}, 29: "*

 * *            "{'source': {insert: [(53, '\\n'), (54, 'if not news.empty:\\n'), (55, '    htmlcode "*

 * *            '+= widgets.row(\\n\'), (56, \'        [widgets.h(3, "Top news on \\\'economy\\\' '*

 * *            'keyword (source: Newsapi)") + news.to_html()]\\n\'), (57, \'    )\\n\'), (58, \'    '*

 * *            "\\n')], delete: [55,  […]*

```diff
@@ -140,25 +140,36 @@
                 "overview = openbb.economy.overview()\n",
                 "overview.set_index(list(overview.columns[0]), inplace=True)\n",
                 "overview = OpenBBFigure.to_table(overview, print_index=True, width=600)\n",
                 "\n",
                 "futures = openbb.economy.futures()\n",
                 "futures.set_index(list(futures.columns[0]), inplace=True)\n",
                 "futures[\"%Chg\"] = futures[\"%Chg\"].apply(lambda x: float(f\"{x:.2f}\"))\n",
-                "futures_fig = OpenBBFigure.to_table(futures, print_index=True)\n",
-                "\n",
-                "news = openbb.news(\"economy\")\n",
-                "news.columns = news.columns.str.title()\n",
-                "news[\"Title\"] = news.apply(lambda x: f'<a href=\"{x[\"Link\"]}\">{x[\"Title\"]}</a>', axis=1)\n",
-                "news = news[[\"Title\", \"Published\"]]\n",
-                "news[\"Published\"] = pd.to_datetime(news[\"Published\"]).dt.strftime(\"%Y-%m-%d %H:%M\")\n",
-                "news.set_index(\"Published\", inplace=True)\n",
+                "futures_fig = OpenBBFigure.to_table(futures, print_index=True)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "351d0451",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "try:\n",
+                "    news = openbb.news(\"economy\")\n",
+                "    news.columns = news.columns.str.title()\n",
+                "    news[\"Title\"] = news.apply(lambda x: f'<a href=\"{x[\"Link\"]}\">{x[\"Title\"]}</a>', axis=1)\n",
+                "    news = news[[\"Title\", \"Published\"]]\n",
+                "    news[\"Published\"] = pd.to_datetime(news[\"Published\"]).dt.strftime(\"%Y-%m-%d %H:%M\")\n",
+                "    news.set_index(\"Published\", inplace=True)\n",
                 "\n",
-                "news = OpenBBFigure.to_table(news, print_index=True, columnwidth=[1.3, 7], width=1100)\n",
-                "news.update_layout(clickmode=\"event+select\")"
+                "    news = OpenBBFigure.to_table(news, print_index=True, columnwidth=[1.3, 7], width=1100)\n",
+                "    news.update_layout(clickmode=\"event+select\")\n",
+                "except:\n",
+                "    news = pd.DataFrame()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "64729474",
             "metadata": {},
@@ -649,17 +660,20 @@
                 "    [widgets.h(3, \"Commodities (source: WSJ)\") + futures_fig.to_html()]\n",
                 "    + [\n",
                 "        widgets.h(3, \"Real-time sector performance (source: Alphavantage)\")\n",
                 "        + rtps_data.to_html().replace(\"table\", 'table style=\"display:inline\"')\n",
                 "    ]\n",
                 ")\n",
                 "htmlcode += widgets.row([chart_0])\n",
-                "htmlcode += widgets.row(\n",
-                "    [widgets.h(3, \"Top news on 'economy' keyword (source: Newsapi)\") + news.to_html()]\n",
-                ")\n",
+                "\n",
+                "if not news.empty:\n",
+                "    htmlcode += widgets.row(\n",
+                "        [widgets.h(3, \"Top news on 'economy' keyword (source: Newsapi)\") + news.to_html()]\n",
+                "    )\n",
+                "    \n",
                 "body += widgets.add_tab(\"SUMMARY\", htmlcode)\n",
                 "\n",
                 "# Events\n",
                 "htmlcode = widgets.row([widgets.h(3, \"Economic calendars (source: investing.com)\")])\n",
                 "htmlcode += widgets.row([widgets.h(3, \"United States\") + events_1.to_html()])\n",
                 "htmlcode += widgets.row(\n",
                 "    [widgets.h(3, \"Select European Countries\") + events_2.to_html()]\n",
@@ -734,15 +748,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.9.13"
         },
         "vscode": {
             "interpreter": {
                 "hash": "381a209f752e9104bff95ec5e80679ea2e476866b80e4326f1ee6b7658af6049"
             }
         }
     },
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/equity.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/equity.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967241557213056%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(1, '\\n'), (2, 'if expiry_dates:\\n'), (3, '    exp = "*

 * *            "expiry_dates[0]\\n'), (4, '    option_chain = openbb.stocks.options.chains(symbol, "*

 * *            'expiration=exp)\\n\'), (5, \'    current_price = float(ticker_data["Adj '*

 * *            'Close"][-1])\')], delete: [3, 2, 1]}}, 23: {\'source\': {insert: [(0, \'if '*

 * *            "expiry_dates:\\n'), (1, '    vol_chart = openbb.stocks.options.vol(\\n'), (2, "*

 * *            "'        option_chain, current_pric […]*

```diff
@@ -321,47 +321,42 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "bd79195c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "expiry_dates = openbb.stocks.options.expirations(symbol)\n",
-                "exp = expiry_dates[0]\n",
-                "option_chain = openbb.stocks.options.chains(symbol, expiration=exp)\n",
-                "current_price = float(ticker_data[\"Adj Close\"][-1])"
+                "\n",
+                "if expiry_dates:\n",
+                "    exp = expiry_dates[0]\n",
+                "    option_chain = openbb.stocks.options.chains(symbol, expiration=exp)\n",
+                "    current_price = float(ticker_data[\"Adj Close\"][-1])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ad6d0c24",
             "metadata": {},
             "outputs": [],
             "source": [
-                "vol_chart = openbb.stocks.options.vol(\n",
-                "    option_chain, current_price, symbol, exp, external_axes=True\n",
-                ")\n",
+                "if expiry_dates:\n",
+                "    vol_chart = openbb.stocks.options.vol(\n",
+                "        option_chain, current_price, symbol, exp, external_axes=True\n",
+                "    )\n",
                 "\n",
-                "if vol_chart:\n",
-                "    vol_chart = vol_chart.to_html()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "be2d1e3a",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "voi_chart = openbb.stocks.options.voi(\n",
-                "    option_chain, current_price, symbol, exp, external_axes=True\n",
-                ")\n",
+                "    if vol_chart:\n",
+                "        vol_chart = vol_chart.to_html()\n",
+                "\n",
+                "    voi_chart = openbb.stocks.options.voi(\n",
+                "        option_chain, current_price, symbol, exp, external_axes=True\n",
+                "    )\n",
                 "\n",
-                "if voi_chart:\n",
-                "    voi_chart = voi_chart.to_html()"
+                "    if voi_chart:\n",
+                "        voi_chart = voi_chart.to_html()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "324e2d4b-b2f6-4da3-bac4-ef785ad4e436",
             "metadata": {},
@@ -1205,23 +1200,25 @@
                 "    )\n",
                 "except:\n",
                 "    pass\n",
                 "\n",
                 "body += widgets.add_tab(\"Fundamental Analysis\", htmlcode)\n",
                 "\n",
                 "htmlcode = widgets.row([widgets.h(3, \"Put to call ratio\") + (pcr_chart or \"\")])\n",
-                "htmlcode += widgets.row(\n",
-                "    [widgets.h(3, \"Option Volume for closest expiry date\") + (vol_chart or \"\")]\n",
-                ")\n",
-                "htmlcode += widgets.row(\n",
-                "    [\n",
-                "        widgets.h(3, \"Volume and Open Interest for closest expiry date\")\n",
-                "        + (voi_chart or \"\")\n",
-                "    ]\n",
-                ")\n",
+                "\n",
+                "if expiry_dates:\n",
+                "    htmlcode += widgets.row(\n",
+                "        [widgets.h(3, \"Option Volume for closest expiry date\") + (vol_chart or \"\")]\n",
+                "    )\n",
+                "    htmlcode += widgets.row(\n",
+                "        [\n",
+                "            widgets.h(3, \"Volume and Open Interest for closest expiry date\")\n",
+                "            + (voi_chart or \"\")\n",
+                "        ]\n",
+                "    )\n",
                 "\n",
                 "body += widgets.add_tab(\"Options\", htmlcode)\n",
                 "\n",
                 "htmlcode = widgets.row([net_short_position or \"\"])\n",
                 "htmlcode += widgets.row([price_vs_short_interest or \"\"])\n",
                 "# htmlcode += widgets.row([dark_pools])\n",
                 "body += widgets.add_tab(\"Dark Pool and Shorts\", htmlcode)\n",
@@ -1381,15 +1378,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.9"
+            "version": "3.9.13"
         },
         "vscode": {
             "interpreter": {
                 "hash": "af870c0f9615f5bb08692efcc9bf540319fe60e6793056508a4dab09c9fa8dda"
             }
         }
     },
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/etf.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/etf.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/floppy-disc.png` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/floppy-disc.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/forecast.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/forex.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/forex.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998604693917194%*

 * *Differences: {"'cells'": "{30: {'source': {insert: [(1, 'try:\\n'), (2, '    news = "*

 * *            'openbb.news(term=ticker).head(10)\\n\'), (4, \'    news["published"] = '*

 * *            'pd.to_datetime(news["published"])\\n\'), (5, \'    news["published"] = '*

 * *            'pd.to_datetime(\\n\'), (6, \'        news["published"], format="%d/%m/%y '*

 * *            '%H:%M:%S"\\n\'), (7, \'    ).dt.strftime("%Y-%m-%d")\\n\'), (8, \'    news = '*

 * *            'news[["published", "title", "link"]]\\n\'), (10, \'    news["link"] = '*

 * *   […]*

```diff
@@ -464,27 +464,28 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "fc31624a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# latest news\n",
+                "try:\n",
+                "    news = openbb.news(term=ticker).head(10)\n",
                 "\n",
-                "news = openbb.news(term=ticker).head(10)\n",
-                "\n",
-                "news[\"published\"] = pd.to_datetime(news[\"published\"])\n",
-                "news[\"published\"] = pd.to_datetime(\n",
-                "    news[\"published\"], format=\"%d/%m/%y %H:%M:%S\"\n",
-                ").dt.strftime(\"%Y-%m-%d\")\n",
-                "news = news[[\"published\", \"title\", \"link\"]]\n",
-                "\n",
-                "news[\"link\"] = news[\"link\"].apply(lambda x: f'<a href=\"{x}\">{x}</a>')\n",
-                "news = news.set_index(\"published\")\n",
-                "news.sort_index()\n",
-                "news"
+                "    news[\"published\"] = pd.to_datetime(news[\"published\"])\n",
+                "    news[\"published\"] = pd.to_datetime(\n",
+                "        news[\"published\"], format=\"%d/%m/%y %H:%M:%S\"\n",
+                "    ).dt.strftime(\"%Y-%m-%d\")\n",
+                "    news = news[[\"published\", \"title\", \"link\"]]\n",
+                "\n",
+                "    news[\"link\"] = news[\"link\"].apply(lambda x: f'<a href=\"{x}\">{x}</a>')\n",
+                "    news = news.set_index(\"published\")\n",
+                "    news.sort_index()\n",
+                "except:\n",
+                "    news = pd.DataFrame()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ac501a32-124d-4d21-aae1-a8d147bb1071",
             "metadata": {},
             "source": [
@@ -648,15 +649,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.9.13"
         },
         "vscode": {
             "interpreter": {
                 "hash": "381a209f752e9104bff95ec5e80679ea2e476866b80e4326f1ee6b7658af6049"
             }
         }
     },
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/templates/portfolio.ipynb` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/templates/portfolio.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widget_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widget_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/report.css` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/report.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/reports/widgets/style.css` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/reports/widgets/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/rich_config.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/rich_config.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/sdk.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/sdk.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/settings_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/settings_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,15 @@
                 set_preference("RICH_STYLE", ns_parser.style)
                 Hub.upload_config(
                     key="RICH_STYLE",
                     value=ns_parser.style,
                     type_="settings",
                     auth_header=get_current_user().profile.get_auth_header(),
                 )
+                console.print("")
             console.print("Colors updated.")
 
     @log_start_end(log=logger)
     def call_theme(self, other_args: List[str]):
         """Process theme command"""
         parser = argparse.ArgumentParser(
             add_help=False,
@@ -323,15 +324,16 @@
                 set_preference("THEME", ns_parser.style)
                 Hub.upload_config(
                     key="chart_table",
                     value=ns_parser.style,
                     type_="terminal_style",
                     auth_header=get_current_user().profile.get_auth_header(),
                 )
-            console.print("Theme updated.")
+                console.print("")
+            console.print("Theme updated.\n")
 
     @log_start_end(log=logger)
     def call_source(self, other_args: List[str]):
         """Process source command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/sources_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/sources_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/backtesting/bt_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/backtesting/bt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/ba_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/ba_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/cboe_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/cboe_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/cboe_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/cboe_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/ca_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/ca_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/finra_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/finra_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/finra_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/finra_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/sec_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/sec_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/sec_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/sec_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/databento_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/databento_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/ark_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/ark_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/ark_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/ark_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/disc_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fidelity_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fidelity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fidelity_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fidelity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/nasdaq_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/shortinterest_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/shortinterest_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/yahoofinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/discovery/yahoofinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/discovery/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/av_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/av_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_static.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_static.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/dcf_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/dcf_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,26 @@
     if len(response_dict) == 0:
         return pd.DataFrame()
 
     risk = pd.DataFrame(
         map(resultGroupMapper("Risk factors"), response_dict[0]["rf_highlights"]),
         columns=["Group", "Good", "Sentence"],
     )
+
+    if risk.empty:
+        response_dict_rf = [x for x in response_dict if x["rf_highlights"] != []]
+        if response_dict_rf != []:
+            risk = pd.DataFrame(
+                map(
+                    resultGroupMapper("Risk factors"),
+                    response_dict_rf[0]["rf_highlights"],
+                ),
+                columns=["Group", "Good", "Sentence"],
+            )
+
     analysis = pd.DataFrame(
         map(
             resultGroupMapper("Discussion and Analysis"),
             response_dict[0]["daa_highlights"],
         ),
         columns=["Group", "Good", "Sentence"],
     )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fa_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,15 +820,15 @@
             "--holder",
             choices=self.SHRS_CHOICES,
             default="institutional",
             help="Table of holders to get",
             dest="holder",
         )
 
-        if other_args and "--holder" not in other_args[0][0] and "-h" not in other_args:
+        if other_args and "--holder" not in other_args[0] and "-h" not in other_args:
             other_args.insert(0, "--holder")
 
         ns_parser = self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
         )
         if ns_parser:
             if ns_parser.ticker:
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fmp_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/fmp_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/market_watch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/market_watch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/polygon_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/polygon_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/polygon_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/gov_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/gov_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/quiverquant_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/quiverquant_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/government/quiverquant_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/government/quiverquant_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/businessinsider_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/businessinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/businessinsider_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/businessinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/insider_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/insider_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/openinsider_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/openinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/openinsider_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/openinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/insider/sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/insider/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/mappings/Mic_Codes.csv` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/mappings/Mic_Codes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/alphaquery_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/alphaquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/alphaquery_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/alphaquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/barchart_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/barchart_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/barchart_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/barchart_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/calculator_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/calculator_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/calculator_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/calculator_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/chartexchange_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/chartexchange_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/chartexchange_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/chartexchange_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/fdscanner_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/fdscanner_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/fdscanner_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/fdscanner_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/hedge/hedge_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/hedge/hedge_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/intrinio_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/intrinio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/intrinio_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/intrinio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/nasdaq_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/op_helpers.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/op_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         expiration: Optional[str] = None,
     ):
         """Constructor"""
         super().__init__(queue)
 
         self.ticker = ticker
         self.prices = pd.DataFrame(columns=["Price", "Chance"])
-        self.selected_date = expiration if expiration else ""
+        self.selected_date = expiration or ""
         self.chain: pd.DataFrame = pd.DataFrame()
         self.full_chain: pd.DataFrame = pd.DataFrame()
 
         self.current_price = 0.0
         # Keeps track of initial source of load so we can use correct commands later
         self.source = ""
 
@@ -169,18 +169,15 @@
         See `BaseController.parse_input()` for details.
         """
         # Filtering out sorting parameters with forward slashes like P/E
         sort_filter = r"((\ -s |\ --sortby ).*?(Vol\/OI)*)"
 
         custom_filters = [sort_filter]
 
-        commands = parse_and_split_input(
-            an_input=an_input, custom_filters=custom_filters
-        )
-        return commands
+        return parse_and_split_input(an_input=an_input, custom_filters=custom_filters)
 
     def set_option_chain(self):
         df = pd.DataFrame()
 
         if self.source == "Tradier":
             df = tradier_model.get_full_option_chain(self.ticker)
 
@@ -198,21 +195,21 @@
             not isinstance(df, pd.DataFrame) and not df
         ):
             console.print("[red]Error loading option chain.[/red]")
             return
         self.full_chain = df.copy(deep=True)
         self.chain = self.full_chain.copy(deep=True)
 
-        console.print("Loaded option chain from", self.source)
+        console.print(f"Loaded option chain from {self.source}\n")
 
     def set_current_price(self):
         if not self.chain.empty:
             if self.source == "Tradier":
                 last_price = tradier_model.get_last_price(self.ticker)
-                self.current_price = last_price if last_price else 0.0
+                self.current_price = last_price or 0.0
             elif self.source == "Nasdaq":
                 self.current_price = nasdaq_model.get_last_price(self.ticker)
             elif self.source == "Intrinio":
                 self.current_price = intrinio_model.get_last_price(self.ticker)
             else:
                 self.current_price = yfinance_model.get_last_price(self.ticker)
 
@@ -355,16 +352,15 @@
             "--max",
             type=float,
             dest="max",
             help="Max price to look at",
             default=-1,
             required="-m" in other_args,
         )
-        ns_parser = self.parse_known_args_and_warn(parser, other_args)
-        if ns_parser:
+        if ns_parser := self.parse_known_args_and_warn(parser, other_args):
             pars = (
                 {"x_min": ns_parser.min, "x_max": ns_parser.max}
                 if ns_parser.min > 0 and ns_parser.max > 0
                 else {}
             )
 
             calculator_view.view_calculator(
@@ -427,18 +423,17 @@
             dest="calls_only",
             help="Flag to show calls only",
             default=False,
             action="store_true",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
-        )
-        if ns_parser:
+        ):
             if ns_parser.calls_only and ns_parser.puts_only:
                 console.print(
                     "Cannot return puts only and calls only. Either use one or neither."
                 )
             else:
                 fdscanner_view.display_options(
                     limit=ns_parser.limit,
@@ -474,18 +469,17 @@
             help="Start date for plot",
             type=valid_date,
             default=datetime.now() - timedelta(days=366),
             dest="start",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-l")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, export_allowed=EXPORT_BOTH_RAW_DATA_AND_FIGURES
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 alphaquery_view.display_put_call_ratio(
                     symbol=self.ticker,
                     window=ns_parser.length,
                     start_date=ns_parser.start.strftime("%Y-%m-%d"),
                     export=ns_parser.export,
                     sheet_name=" ".join(ns_parser.sheet_name)
@@ -500,18 +494,17 @@
         """Process info command"""
         parser = argparse.ArgumentParser(
             add_help=False,
             formatter_class=argparse.ArgumentDefaultsHelpFormatter,
             prog="info",
             description="Display option data [Source: Barchart.com]",
         )
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 barchart_view.print_options_data(
                     symbol=self.ticker,
                     export=ns_parser.export,
                     sheet_name=" ".join(ns_parser.sheet_name)
                     if ns_parser.sheet_name
                     else None,
@@ -575,18 +568,17 @@
             dest="limit",
             default=20,
             type=int,
             help="Limit of raw data rows to display",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-s")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_BOTH_RAW_DATA_AND_FIGURES
-        )
-        if ns_parser:
+        ):
             if self.ticker or "--chain" in other_args:
                 if self.selected_date or "--chain" in other_args:
                     if (
                         not self.chain.empty
                         and (
                             (
                                 ns_parser.put
@@ -648,24 +640,23 @@
             description="Load a ticker into option menu",
         )
         parser.add_argument(
             "-t",
             "--ticker",
             action="store",
             dest="ticker",
-            required="-h" not in other_args,
+            required="-h" not in other_args and "--help" not in other_args,
             help="Stock ticker",
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-t")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser,
             other_args,
-        )
-        if ns_parser:
+        ):
             self.ticker = ns_parser.ticker.upper()
             self.source = ns_parser.source
 
             self.set_option_chain()
             self.set_current_price()
             self.set_expiry_dates()
             self.selected_date = ""
@@ -712,16 +703,15 @@
         if other_args and "-" not in other_args[0][0]:
             first_int = int(other_args[0].split("-")[0])
             if first_int > 2000:
                 other_args.insert(0, "-d")
             else:
                 other_args.insert(0, "-i")
 
-        ns_parser = self.parse_known_args_and_warn(parser, other_args)
-        if ns_parser:
+        if ns_parser := self.parse_known_args_and_warn(parser, other_args):
             if self.ticker:
                 # Print possible expiry dates
                 if ns_parser.index == -1 and not ns_parser.date:
                     display_expiry_dates(self.expiry_dates)
                 # Set expiry date with date argument
                 elif ns_parser.date:
                     if ns_parser.date in self.expiry_dates:
@@ -778,22 +768,21 @@
             dest="chain_id",
             type=str,
             help="Option symbol",
             default=None,
         )
         if other_args and "-" not in other_args[0][0]:
             other_args.insert(0, "-s")
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser,
             other_args,
             EXPORT_BOTH_RAW_DATA_AND_FIGURES,
             raw=True,
             limit=10,
-        )
-        if ns_parser:
+        ):
             if not self.ticker and ns_parser.chain_id is None:
                 console.print("No ticker loaded. First use `load <ticker>`")
                 return
             if not self.selected_date and ns_parser.chain_id is None:
                 console.print("No expiry loaded. First use `exp <expiry date>`")
                 return
             if (
@@ -899,31 +888,30 @@
             default=-1,
             help="maximum strike price to consider.",
         )
         parser.add_argument(
             "-d",
             "--display",
             dest="to_display",
-            default=",".join(list(self.chain)) if not self.chain.empty else [],
+            default=[] if self.chain.empty else ",".join(list(self.chain)),
             type=str,
             help="Columns to display",
         )
         parser.add_argument(
             "-e",
             "--expiration",
             dest="exp",
             type=str,
             choices=self.expiry_dates + [""],
             help="Select expiration date (YYYY-MM-DD)",
             default="",
         )
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_RAW_DATA_ALLOWED
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 if ns_parser.exp:
                     if ns_parser.exp in self.expiry_dates:
                         self.selected_date = ns_parser.exp
                         self.chain = self.full_chain[
                             self.full_chain["expiration"] == self.selected_date
                         ]
@@ -1010,21 +998,20 @@
             "--expiration",
             dest="exp",
             type=str,
             choices=self.expiry_dates + [""],
             help="Select expiration date (YYYY-MM-DD)",
             default="",
         )
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser,
             other_args,
             export_allowed=EXPORT_BOTH_RAW_DATA_AND_FIGURES,
             raw=True,
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 if ns_parser.exp:
                     if ns_parser.exp in self.expiry_dates:
                         self.selected_date = ns_parser.exp
                         self.chain = self.full_chain[
                             self.full_chain["expiration"] == self.selected_date
                         ]
@@ -1096,18 +1083,17 @@
             "--expiration",
             dest="exp",
             type=str,
             choices=self.expiry_dates + [""],
             help="Select expiration date (YYYY-MM-DD)",
             default="",
         )
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_BOTH_RAW_DATA_AND_FIGURES, raw=True
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 if ns_parser.exp:
                     if ns_parser.exp in self.expiry_dates:
                         self.selected_date = ns_parser.exp
                         self.chain = self.full_chain[
                             self.full_chain["expiration"] == self.selected_date
                         ]
@@ -1186,21 +1172,20 @@
             "--expiration",
             dest="exp",
             type=str,
             choices=self.expiry_dates + [""],
             help="Select expiration date (YYYY-MM-DD)",
             default="",
         )
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser,
             other_args,
             raw=True,
             export_allowed=EXPORT_BOTH_RAW_DATA_AND_FIGURES,
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 if ns_parser.exp:
                     if ns_parser.exp in self.expiry_dates:
                         self.selected_date = ns_parser.exp
                         self.chain = self.full_chain[
                             self.full_chain["expiration"] == self.selected_date
                         ]
@@ -1281,18 +1266,17 @@
             type=str,
             choices=self.plot_custom_choices,
             dest="custom",
             default=None,
             help="Choose from already created graphs",
         )
 
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, EXPORT_ONLY_FIGURES_ALLOWED
-        )
-        if ns_parser:
+        ):
             if self.ticker:
                 if self.selected_date:
                     if (
                         ns_parser.x is None or ns_parser.y is None
                     ) and ns_parser.custom is None:
                         console.print(
                             "Please submit an X and Y value, or select a preset."
@@ -1327,18 +1311,17 @@
             default="IV",
             dest="z",
             choices=["IV", "OI", "LP"],
             type=str,
             help="The data for the Z axis",
         )
 
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, export_allowed=EXPORT_ONLY_FIGURES_ALLOWED
-        )
-        if ns_parser:
+        ):
             yfinance_view.display_vol_surface(
                 self.ticker,
                 export=ns_parser.export,
                 z=ns_parser.z,
             )
 
     @log_start_end(log=logger)
@@ -1395,18 +1378,17 @@
             "--all",
             dest="all",
             action="store_true",
             default=False,
             help="Whether to show all greeks.",
         )
 
-        ns_parser = self.parse_known_args_and_warn(
+        if ns_parser := self.parse_known_args_and_warn(
             parser, other_args, export_allowed=EXPORT_ONLY_FIGURES_ALLOWED
-        )
-        if ns_parser:
+        ):
             if not self.ticker:
                 console.print("No ticker loaded. First use `load <ticker>`")
             elif not self.selected_date:
                 console.print("No expiry loaded. First use `exp {expiry date}`")
             else:
                 opt_type = -1 if ns_parser.put else 1
                 yfinance_view.show_greeks(
@@ -1452,20 +1434,18 @@
             description="Get full option chain at a given end of day.",
         )
         parser.add_argument(
             "-d",
             "--date",
             type=valid_date,
             dest="date",
-            help="Date to get option chain for.  Format YYYY-MM-DD",
-            required="-h" not in other_args,
+            help="Date to get option chain for. Format YYYY-MM-DD",
+            required="-h" not in other_args and "--help" not in other_args,
         )
 
-        ns_parser = self.parse_known_args_and_warn(parser, other_args)
-
-        if ns_parser:
+        if ns_parser := self.parse_known_args_and_warn(parser, other_args):
             if not self.ticker:
                 console.print("No ticker loaded. First use `load <ticker>`")
                 return
             self.full_chain = intrinio_model.get_full_chain_eod(
                 self.ticker, datetime.strftime(ns_parser.date, "%Y-%m-%d")
             )
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_sdk_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_sdk_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
         output = nasdaq_model.option_expirations(symbol)
     if source == "intrinio":
         output = intrinio_model.get_expiration_dates(symbol)
 
     if (output := None) is None:
         logger.info("Invalid Source or Symbol")
         console.print("Invalid Source or Symbol")
-        return pd.DataFrame()
+        return []
 
     return output
 
 
 @log_start_end(log=logger)
 def hist(
     symbol: str,
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/options_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/options_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/screener_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/syncretism_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/syncretism_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/screen/syncretism_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/screen/syncretism_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/tradier_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/tradier_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/tradier_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/tradier_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/yfinance_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/options/yfinance_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/options/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/beta_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/beta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/beta_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/beta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/factors_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/factors_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/factors_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/factors_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/research/res_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/research/res_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/screener/screener_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/screener/screener_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stock_statics.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stock_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/stocks_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/stocks_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finbrain_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finbrain_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finviz_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/finviz_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/rsp_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/rsp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/rsp_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/rsp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/tradingview_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/tradingview_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/technical_analysis/tradingview_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/technical_analysis/tradingview_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/bursa_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/bursa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/bursa_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/bursa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/tradinghours_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/tradinghours_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/stocks/tradinghours/tradinghours_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/stocks/tradinghours/tradinghours_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/terminal_controller.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/terminal_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/terminal_helper.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/terminal_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     console.print(
         "We are always eager to welcome new contributors and you can find our open jobs here:\n"
         "[cmds]https://www.openbb.co/company/careers#open-roles[/cmds]\n"
     )
 
     console.print(
         "Join us           : [cmds]https://openbb.co/discord[/cmds]\n"
-        "Follow us         : [cmds]https://twitter.com/openbb_finance[/cmds]\n"
+        "Follow us         : [cmds]https://openbb.co/twitter[/cmds]\n"
         "Ask support       : [cmds]https://openbb.co/support[/cmds]\n"
         "Request a feature : [cmds]https://openbb.co/request-a-feature[/cmds]\n"
     )
 
     console.print(
         "[bold]Fill in our 2-minute survey so we better understand how we can improve the OpenBB Terminal "
         "at [cmds]https://openbb.co/survey[/cmds][/bold]\n"
@@ -125,82 +125,93 @@
     if completed_process.returncode != 0:
         return completed_process.returncode
 
     return 0
 
 
 def open_openbb_documentation(
-    path, url="https://my.openbb.dev/app/terminal", command=None, arg_type=""
+    path,
+    url="https://my.openbb.dev/app/terminal",
+    command=None,
+    arg_type="",
 ):
     """Opens the documentation page based on your current location within the terminal. Make exceptions for menus
     that are considered 'common' by adjusting the path accordingly."""
     if path == "/" and command is None:
-        path = "/guides"
+        path = "/usage?path=/usage/basics"
         command = ""
     elif "keys" in path:
-        path = "/usage?full=1&path=/guides/api-keys"
+        path = "/usage?path=/usage/guides/api-keys"
         command = ""
     elif "settings" in path:
-        path = "/usage?path=/guides/customizing-the-terminal"
+        path = "/usage?path=/usage/guides/customizing-the-terminal"
         command = ""
     elif "featflags" in path:
-        path = "/usage?path=/guides/customizing-the-terminal"
+        path = "/usage?path=/usage/guides/customizing-the-terminal#using-the-feature-flags-menu"
         command = ""
     elif "sources" in path:
-        path = "/usage?path=/guides/changing-sources"
+        path = "/usage?path=/usage/guides/changing-sources"
         command = ""
-    elif "params" in path:
-        path = "/usage?path=/intros/portfolio/po"
+    elif "account" in path:
+        path = "/usage?path=/usage/guides/basics"
         command = ""
     else:
         if arg_type == "command":  # user passed a command name
-            path = f"/reference?path={path}"
+            if command in ["settings", "featflags"]:
+                path = "/usage?path=/usage/guides/customizing-the-terminal"
+                command = ""
+            else:
+                path = f"/reference?path={path}"
         elif arg_type == "menu":  # user passed a menu name
             if command in ["ta", "ba", "qa"]:
                 menu = path.split("/")[-2]
-                path = f"/usage?path=/intros/common/{menu}"
+                path = f"/usage?path=/usage/intros/common/{menu}"
             elif command == "forecast":
                 command = ""
-                path = "/usage?path=/intros/forecast"
+                path = "/usage?path=/usage/intros/forecast"
             else:
-                path = f"/usage?path=/intros/{path}"
+                path = f"/usage?path=/usage/intros/{path}"
         else:  # user didn't pass argument and is in a menu
             menu = path.split("/")[-2]
             path = (
-                f"/usage?path=/intros/common/{menu}"
+                f"/usage?path=/usage/intros/common/{menu}"
                 if menu in ["ta", "ba", "qa"]
-                else f"/usage?path=/intros/{path}"
+                else f"/usage?path=/usage/intros/{path}"
             )
 
     if command:
         if command == "keys":
-            path = "/usage?full=1&path=/guides/api-keys"
+            path = "/usage?path=/usage/guides/api-keys"
             command = ""
         elif "settings" in path or "featflags" in path:
-            path = "/usage?path=/guides/customizing-the-terminal"
+            path = "/usage?path=/usage/guides/customizing-the-terminal"
             command = ""
         elif "sources" in path:
-            path = "/usage?path=/guides/changing-sources"
+            path = "/usage?path=/usage/guides/changing-sources"
             command = ""
         elif command in ["record", "stop", "exe"]:
-            path = "/usage?path=/guides/scripts-and-routines"
+            path = "/usage?path=/usage/guides/scripts-and-routines"
+            command = ""
+        elif command == "sources":
+            path = "/usage?path=/usage/guides/changing-sources"
             command = ""
         elif command in [
             "intro",
             "about",
             "support",
             "survey",
             "update",
             "wiki",
             "news",
+            "account",
         ]:
             path = "/guides"
             command = ""
         elif command in ["ta", "ba", "qa"]:
-            path = f"/guides?path=/intros/common/{command}"
+            path = f"/usage?path=/usage/intros/common/{command}"
             command = ""
 
         path += command
 
     full_url = f"{url}{path.replace('//', '/')}"
 
     if full_url[-1] == "/":
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/openbb_terminal/thought_of_the_day.py` & `openbb_nightly-3.0.0rc1.dev20230411/openbb_terminal/thought_of_the_day.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/pyproject.toml` & `openbb_nightly-3.0.0rc1.dev20230411/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "openbb-nightly"
-version = "3.0.0rc1.dev20230410"
+version = "3.0.0rc1.dev20230411"
 description = "Investment Research for Everyone, Anywhere."
 license = "MIT"
 authors = ["Didier Rodrigues Lopes"]
 packages = [
     { include = "openbb_terminal" },
 ]
-include = ["terminal.py"]
+include = ["terminal.py", "openbb_terminal/.env"]
 readme = "website/pypi.md"
 homepage = "https://openbb.co"
 repository = "https://github.com/OpenBB-finance/OpenBBTerminal"
 documentation = "https://docs.openbb.co/sdk"
 
 [tool.poetry.scripts]
 openbb = 'terminal:main'
```

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/terminal.py` & `openbb_nightly-3.0.0rc1.dev20230411/terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/website/pypi.md` & `openbb_nightly-3.0.0rc1.dev20230411/website/pypi.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.0rc1.dev20230410/PKG-INFO` & `openbb_nightly-3.0.0rc1.dev20230411/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 3.0.0rc1.dev20230410
+Version: 3.0.0rc1.dev20230411
 Summary: Investment Research for Everyone, Anywhere.
 Home-page: https://openbb.co
 License: MIT
 Author: Didier Rodrigues Lopes
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

