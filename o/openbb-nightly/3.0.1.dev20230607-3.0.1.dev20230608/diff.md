# Comparing `tmp/openbb_nightly-3.0.1.dev20230607.tar.gz` & `tmp/openbb_nightly-3.0.1.dev20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-3.0.1.dev20230607.tar", max compression
+gzip compressed data, was "openbb_nightly-3.0.1.dev20230608.tar", max compression
```

## Comparing `openbb_nightly-3.0.1.dev20230607.tar` & `openbb_nightly-3.0.1.dev20230608.tar`

### file list

```diff
@@ -1,948 +1,948 @@
--rw-r--r--   0        0        0     1073 2023-06-07 00:09:56.017373 openbb_nightly-3.0.1.dev20230607/LICENSE
--rw-r--r--   0        0        0      243 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/__init__.py
--rw-r--r--   0        0        0    22105 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/account_controller.py
--rw-r--r--   0        0        0     1769 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/account_view.py
--rw-r--r--   0        0        0      419 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/show_prompt.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/__init__.py
--rw-r--r--   0        0        0     3131 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/alt_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/countries.txt
--rw-r--r--   0        0        0     9347 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_controller.py
--rw-r--r--   0        0        0     5388 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_model.py
--rw-r--r--   0        0        0     8586 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_view.py
--rw-r--r--   0        0        0     1070 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/hackernews_model.py
--rw-r--r--   0        0        0     1087 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/hackernews_view.py
--rw-r--r--   0        0        0     6752 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/github_model.py
--rw-r--r--   0        0        0     3968 2023-06-07 00:09:56.221372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/github_view.py
--rw-r--r--   0        0        0     8656 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/oss_controller.py
--rw-r--r--   0        0        0     4437 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/runa_model.py
--rw-r--r--   0        0        0     4018 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/runa_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/__init__.py
--rw-r--r--   0        0        0     9030 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/landRegistry_model.py
--rw-r--r--   0        0        0     3309 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/landRegistry_view.py
--rw-r--r--   0        0        0     8108 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/realestate_controller.py
--rw-r--r--   0        0        0     2865 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/base_helpers.py
--rw-r--r--   0        0        0       93 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0     1198 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finbrain_model.py
--rw-r--r--   0        0        0     4401 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1335 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     1861 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3329 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/google_model.py
--rw-r--r--   0        0        0     7118 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/google_view.py
--rw-r--r--   0        0        0     5524 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
--rw-r--r--   0        0        0    18297 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_model.py
--rw-r--r--   0        0        0    10170 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_view.py
--rw-r--r--   0        0        0     3239 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
--rw-r--r--   0        0        0     2898 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
--rw-r--r--   0        0        0     6160 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/twitter_model.py
--rw-r--r--   0        0        0     5870 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/twitter_view.py
--rw-r--r--   0        0        0     4956 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/biztoc_model.py
--rw-r--r--   0        0        0     2341 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/biztoc_view.py
--rw-r--r--   0        0        0     4142 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/common_model.py
--rw-r--r--   0        0        0     3634 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/feedparser_model.py
--rw-r--r--   0        0        0     1442 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/feedparser_view.py
--rw-r--r--   0        0        0     1435 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/news_sdk_helper.py
--rw-r--r--   0        0        0     2639 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/newsapi_model.py
--rw-r--r--   0        0        0     1465 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/newsapi_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    19923 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0    32308 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/qa_view.py
--rw-r--r--   0        0        0     3226 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/rolling_model.py
--rw-r--r--   0        0        0    10790 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/rolling_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/__init__.py
--rw-r--r--   0        0        0     2993 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/custom_indicators_model.py
--rw-r--r--   0        0        0     4272 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/custom_indicators_view.py
--rw-r--r--   0        0        0     6427 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/momentum_model.py
--rw-r--r--   0        0        0    12480 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/momentum_view.py
--rw-r--r--   0        0        0     4179 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/overlap_model.py
--rw-r--r--   0        0        0     4430 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/overlap_view.py
--rw-r--r--   0        0        0     1453 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/ta_helpers.py
--rw-r--r--   0        0        0     1819 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/trend_indicators_model.py
--rw-r--r--   0        0        0     2621 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/trend_indicators_view.py
--rw-r--r--   0        0        0    19962 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volatility_model.py
--rw-r--r--   0        0        0    10005 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volatility_view.py
--rw-r--r--   0        0        0     2614 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volume_model.py
--rw-r--r--   0        0        0     3806 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volume_view.py
--rw-r--r--   0        0        0     7577 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/ultima_newsmonitor_model.py
--rw-r--r--   0        0        0     4870 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/ultima_newsmonitor_view.py
--rw-r--r--   0        0        0     2634 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/config_terminal.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/__init__.py
--rw-r--r--   0        0        0     9829 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/completer/choices.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/config/__init__.py
--rw-r--r--   0        0        0     1180 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/config/paths.py
--rw-r--r--   0        0        0     2650 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/config/paths_helper.py
--rw-r--r--   0        0        0     9830 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/README.md
--rw-r--r--   0        0        0     2081 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/controllers.json
--rw-r--r--   0        0        0    23202 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/integration_controller.py
--rw-r--r--   0        0        0    20084 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/integration_test_coverage.py
--rw-r--r--   0        0        0     3389 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/__init__.py
--rw-r--r--   0        0        0     3904 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/log_sender.py
--rw-r--r--   0        0        0     3744 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/logging_clock.py
--rw-r--r--   0        0        0     3495 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/s3_sender.py
--rw-r--r--   0        0        0      166 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/constants.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/__init__.py
--rw-r--r--   0        0        0      524 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/common.py
--rw-r--r--   0        0        0      631 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/custom_logger.py
--rw-r--r--   0        0        0      979 2023-06-07 00:09:56.225372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/directories.py
--rw-r--r--   0        0        0      841 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/expired_files.py
--rw-r--r--   0        0        0     5239 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/formatter_with_exceptions.py
--rw-r--r--   0        0        0     6058 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4200 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/settings.py
--rw-r--r--   0        0        0     1818 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/settings_logger.py
--rw-r--r--   0        0        0      396 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/user_logger.py
--rw-r--r--   0        0        0      627 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/base_model.py
--rw-r--r--   0        0        0      818 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/credentials_model.py
--rw-r--r--   0        0        0     3708 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/preferences_model.py
--rw-r--r--   0        0        0     2041 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/profile_model.py
--rw-r--r--   0        0        0     1230 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/sources_model.py
--rw-r--r--   0        0        0     2922 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/system_model.py
--rw-r--r--   0        0        0      634 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/user_model.py
--rw-r--r--   0        0        0      200 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/__init__.py
--rw-r--r--   0        0        0   418780 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/assets/Terminal_icon.png
--rw-r--r--   0        0        0    14244 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/backend.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/config/__init__.py
--rw-r--r--   0        0        0     7156 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/config/openbb_styles.py
--rw-r--r--   0        0        0     3132 2023-06-07 00:09:56.229372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/no_import.py
--rw-r--r--   0        0        0  4433681 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly.html
--rw-r--r--   0        0        0    63492 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_helper.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/__init__.py
--rw-r--r--   0        0        0     6724 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/base.py
--rw-r--r--   0        0        0    11370 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/data_classes.py
--rw-r--r--   0        0        0     8004 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    18320 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3339 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5683 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6844 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3429 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    20601 2023-06-07 00:09:56.257372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/ta_class.py
--rw-r--r--   0        0        0   711999 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/table.html
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/scripts/__init__.py
--rw-r--r--   0        0        0     7775 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/scripts/sdk_audit.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/__init__.py
--rw-r--r--   0        0        0      450 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/__init__.py
--rw-r--r--   0        0        0     2660 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
--rw-r--r--   0        0        0    24817 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
--rw-r--r--   0        0        0     1513 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
--rw-r--r--   0        0        0     2365 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
--rw-r--r--   0        0        0     5128 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
--rw-r--r--   0        0        0    18025 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
--rw-r--r--   0        0        0      761 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/__init__.py
--rw-r--r--   0        0        0     4308 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/alt_sdk_model.py
--rw-r--r--   0        0        0    44505 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/crypto_sdk_model.py
--rw-r--r--   0        0        0     4889 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
--rw-r--r--   0        0        0     7830 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/economy_sdk_model.py
--rw-r--r--   0        0        0     2496 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/etf_sdk_model.py
--rw-r--r--   0        0        0     3515 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
--rw-r--r--   0        0        0     8550 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/forecast_sdk_model.py
--rw-r--r--   0        0        0     4386 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/forex_sdk_model.py
--rw-r--r--   0        0        0     1530 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/funds_sdk_model.py
--rw-r--r--   0        0        0     1067 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/futures_sdk_model.py
--rw-r--r--   0        0        0     3725 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/keys_sdk_model.py
--rw-r--r--   0        0        0    10046 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
--rw-r--r--   0        0        0     4603 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/qa_sdk_model.py
--rw-r--r--   0        0        0    31836 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/stocks_sdk_model.py
--rw-r--r--   0        0        0     7229 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/ta_sdk_model.py
--rw-r--r--   0        0        0    11588 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/sdk_helpers.py
--rw-r--r--   0        0        0    19897 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/sdk_init.py
--rw-r--r--   0        0        0    44090 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map.csv
--rw-r--r--   0        0        0     2801 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map_forecasting.csv
--rw-r--r--   0        0        0     1301 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map_optimization.csv
--rw-r--r--   0        0        0     6971 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trailmap.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/__init__.py
--rw-r--r--   0        0        0     1017 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/banner.txt
--rw-r--r--   0        0        0      602 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/constants.py
--rw-r--r--   0        0        0     1000 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/current_system.py
--rw-r--r--   0        0        0     4095 2023-06-07 00:09:56.261372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/current_user.py
--rw-r--r--   0        0        0     1400 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/env_handler.py
--rw-r--r--   0        0        0    22314 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/hub_model.py
--rw-r--r--   0        0        0     6162 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/local_model.py
--rw-r--r--   0        0        0     6205 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/routines_handler.py
--rw-r--r--   0        0        0     3672 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/sdk_session.py
--rw-r--r--   0        0        0     3193 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/session_controller.py
--rw-r--r--   0        0        0     6308 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/session_model.py
--rw-r--r--   0        0        0     2834 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/sources_handler.py
--rw-r--r--   0        0        0     1677 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/utils.py
--rw-r--r--   0        0        0     3011 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sources/utils.py
--rw-r--r--   0        0        0      199 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/README.md
--rw-r--r--   0        0        0       84 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/__init__.py
--rw-r--r--   0        0        0     5303 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/coinbase_helpers.py
--rw-r--r--   0        0        0     2147 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
--rw-r--r--   0        0        0    19295 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_controller.py
--rw-r--r--   0        0        0     4481 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_models.py
--rw-r--r--   0        0        0     1785 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_views.py
--rw-r--r--   0        0        0    30340 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
--rw-r--r--   0        0        0      949 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/README.md
--rw-r--r--   0        0        0     7341 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
--rw-r--r--   0        0        0     2436 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
--rw-r--r--   0        0        0     4813 2023-06-07 00:09:56.265372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coingecko_categories.json
--rw-r--r--   0        0        0   954385 2023-06-07 00:09:56.269372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coingecko_coins.json
--rw-r--r--   0        0        0  2245016 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
--rw-r--r--   0        0        0    31307 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/defillama_dapps.json
--rw-r--r--   0        0        0   107203 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/erc20_coins.json
--rw-r--r--   0        0        0     7255 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/finbrain_coins.json
--rw-r--r--   0        0        0   222978 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/santiment_slugs.json
--rw-r--r--   0        0        0   300253 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
--rw-r--r--   0        0        0     4951 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/dataframe_helpers.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/__init__.py
--rw-r--r--   0        0        0     4537 2023-06-07 00:09:56.277372 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/coindix_model.py
--rw-r--r--   0        0        0     2720 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/coindix_view.py
--rw-r--r--   0        0        0     2629 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
--rw-r--r--   0        0        0     2127 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
--rw-r--r--   0        0        0    31284 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/defi_controller.py
--rw-r--r--   0        0        0     8918 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/graph_model.py
--rw-r--r--   0        0        0     7165 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/graph_view.py
--rw-r--r--   0        0        0     5005 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/llama_model.py
--rw-r--r--   0        0        0     5827 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/llama_view.py
--rw-r--r--   0        0        0     1808 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/smartstake_model.py
--rw-r--r--   0        0        0     3110 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/smartstake_view.py
--rw-r--r--   0        0        0     2882 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/substack_model.py
--rw-r--r--   0        0        0     1090 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/substack_view.py
--rw-r--r--   0        0        0     1947 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
--rw-r--r--   0        0        0     2699 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
--rw-r--r--   0        0        0     9734 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
--rw-r--r--   0        0        0     8022 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/__init__.py
--rw-r--r--   0        0        0     2317 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
--rw-r--r--   0        0        0     1620 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
--rw-r--r--   0        0        0     2116 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
--rw-r--r--   0        0        0     1936 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
--rw-r--r--   0        0        0    10255 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
--rw-r--r--   0        0        0     8161 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
--rw-r--r--   0        0        0    24664 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
--rw-r--r--   0        0        0    10833 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
--rw-r--r--   0        0        0     6352 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
--rw-r--r--   0        0        0     1095 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/__init__.py
--rw-r--r--   0        0        0     7483 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
--rw-r--r--   0        0        0     3009 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
--rw-r--r--   0        0        0     3188 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
--rw-r--r--   0        0        0     2840 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
--rw-r--r--   0        0        0     6439 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
--rw-r--r--   0        0        0     4134 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
--rw-r--r--   0        0        0     6587 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
--rw-r--r--   0        0        0     6638 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
--rw-r--r--   0        0        0    15034 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
--rw-r--r--   0        0        0     9133 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
--rw-r--r--   0        0        0     2332 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
--rw-r--r--   0        0        0    64101 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
--rw-r--r--   0        0        0     1850 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
--rw-r--r--   0        0        0     4340 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
--rw-r--r--   0        0        0    15044 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
--rw-r--r--   0        0        0    11237 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
--rw-r--r--   0        0        0    24480 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
--rw-r--r--   0        0        0    22188 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
--rw-r--r--   0        0        0    25887 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
--rw-r--r--   0        0        0     8762 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
--rw-r--r--   0        0        0     3076 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
--rw-r--r--   0        0        0     2070 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
--rw-r--r--   0        0        0     2508 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
--rw-r--r--   0        0        0     6001 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
--rw-r--r--   0        0        0     3474 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/__init__.py
--rw-r--r--   0        0        0     5562 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nft_controller.py
--rw-r--r--   0        0        0     1664 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
--rw-r--r--   0        0        0     4502 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
--rw-r--r--   0        0        0     2895 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/opensea_model.py
--rw-r--r--   0        0        0     1289 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/opensea_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.281371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/__init__.py
--rw-r--r--   0        0        0    21848 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
--rw-r--r--   0        0        0    11444 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
--rw-r--r--   0        0        0     3393 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
--rw-r--r--   0        0        0     4733 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
--rw-r--r--   0        0        0     1840 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
--rw-r--r--   0        0        0     1266 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
--rw-r--r--   0        0        0    15974 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
--rw-r--r--   0        0        0    10572 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
--rw-r--r--   0        0        0    50168 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
--rw-r--r--   0        0        0     6454 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/shroom_model.py
--rw-r--r--   0        0        0     5953 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/shroom_view.py
--rw-r--r--   0        0        0     4772 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
--rw-r--r--   0        0        0     2088 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/__init__.py
--rw-r--r--   0        0        0     2274 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
--rw-r--r--   0        0        0     2427 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
--rw-r--r--   0        0        0     1464 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinbase_model.py
--rw-r--r--   0        0        0     1342 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinbase_view.py
--rw-r--r--   0        0        0    11841 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
--rw-r--r--   0        0        0     9646 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
--rw-r--r--   0        0        0     6776 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
--rw-r--r--   0        0        0     2278 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
--rw-r--r--   0        0        0     1100 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/glassnode_model.py
--rw-r--r--   0        0        0     4677 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/glassnode_view.py
--rw-r--r--   0        0        0     5936 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/loanscan_model.py
--rw-r--r--   0        0        0     3279 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/loanscan_view.py
--rw-r--r--   0        0        0    55381 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/overview_controller.py
--rw-r--r--   0        0        0    13641 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
--rw-r--r--   0        0        0    21320 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
--rw-r--r--   0        0        0     5346 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/rekt_model.py
--rw-r--r--   0        0        0     2253 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/rekt_view.py
--rw-r--r--   0        0        0     2042 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
--rw-r--r--   0        0        0     7167 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
--rw-r--r--   0        0        0     3126 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
--rw-r--r--   0        0        0     6708 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
--rw-r--r--   0        0        0     3480 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
--rw-r--r--   0        0        0     7635 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
--rw-r--r--   0        0        0     5693 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pyth_model.py
--rw-r--r--   0        0        0      973 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pyth_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26081 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
--rw-r--r--   0        0        0    54572 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/__init__.py
--rw-r--r--   0        0        0     6219 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_controller.py
--rw-r--r--   0        0        0     1357 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_helpers.py
--rw-r--r--   0        0        0     3447 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_model.py
--rw-r--r--   0        0        0     2772 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_view.py
--rw-r--r--   0        0        0    16935 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_prompt_toolkit.py
--rw-r--r--   0        0        0    55138 2023-06-07 00:09:56.285371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
--rw-r--r--   0        0        0  2879534 2023-06-07 00:09:56.305371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
--rw-r--r--   0        0        0   350260 2023-06-07 00:09:56.309371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
--rw-r--r--   0        0        0   607642 2023-06-07 00:09:56.313371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
--rw-r--r--   0        0        0    11988 2023-06-07 00:09:56.313371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
--rw-r--r--   0        0        0   667206 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/tvl.png
--rw-r--r--   0        0        0   465754 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/__init__.py
--rw-r--r--   0        0        0     9035 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/dashboards_controller.py
--rw-r--r--   0        0        0    13578 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/Forecasting.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/__init__.py
--rw-r--r--   0        0        0     3985 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/common_vars.py
--rw-r--r--   0        0        0     4299 2023-06-07 00:09:56.317371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Chains.py
--rw-r--r--   0        0        0     3366 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Correlation.py
--rw-r--r--   0        0        0     8170 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Futures.py
--rw-r--r--   0        0        0    17894 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Indicators.py
--rw-r--r--   0        0        0     7008 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Short_Data.py
--rw-r--r--   0        0        0    13262 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Stocks.py
--rw-r--r--   0        0        0     4795 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/streamlit_helpers.py
--rw-r--r--   0        0        0     1251 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/streamlit_run.py
--rw-r--r--   0        0        0     5481 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/chains.ipynb
--rw-r--r--   0        0        0     6789 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/correlation.ipynb
--rw-r--r--   0        0        0    13930 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/forecast.ipynb
--rw-r--r--   0        0        0    10953 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/futures.ipynb
--rw-r--r--   0        0        0     9421 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/shortdata.ipynb
--rw-r--r--   0        0        0    15315 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/stocks.ipynb
--rw-r--r--   0        0        0     5091 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/decorators.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/__init__.py
--rw-r--r--   0        0        0    83900 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_controller.py
--rw-r--r--   0        0        0     2973 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_helpers.py
--rw-r--r--   0        0        0    18675 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_model.py
--rw-r--r--   0        0        0    20044 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_view.py
--rw-r--r--   0        0        0    20449 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/regression_model.py
--rw-r--r--   0        0        0     6739 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/regression_view.py
--rw-r--r--   0        0        0       77 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/__init__.py
--rw-r--r--   0        0        0    10230 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/alphavantage_model.py
--rw-r--r--   0        0        0    12117 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/alphavantage_view.py
--rw-r--r--   0        0        0     1890 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/commodity_model.py
--rw-r--r--   0        0        0     1569 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/commodity_view.py
--rw-r--r--   0        0        0      909 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
--rw-r--r--   0        0        0    21218 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/cpi.csv
--rw-r--r--   0        0        0    10355 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/harmonized_cpi.csv
--rw-r--r--   0        0        0    28404 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/econdb_model.py
--rw-r--r--   0        0        0     8027 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/econdb_view.py
--rw-r--r--   0        0        0    90104 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/economy_controller.py
--rw-r--r--   0        0        0     3436 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/economy_helpers.py
--rw-r--r--   0        0        0     8043 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/finviz_model.py
--rw-r--r--   0        0        0     3837 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/finviz_view.py
--rw-r--r--   0        0        0     9940 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/fred_model.py
--rw-r--r--   0        0        0     9124 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/fred_view.py
--rw-r--r--   0        0        0     6972 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/nasdaq_model.py
--rw-r--r--   0        0        0     3293 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/nasdaq_view.py
--rw-r--r--   0        0        0    38618 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/oecd_model.py
--rw-r--r--   0        0        0    28284 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/oecd_view.py
--rw-r--r--   0        0        0     3768 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/plot_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    28433 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1218 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/sdk_helpers.py
--rw-r--r--   0        0        0    12870 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/wsj_model.py
--rw-r--r--   0        0        0     4673 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/wsj_view.py
--rw-r--r--   0        0        0    30415 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/yfinance_model.py
--rw-r--r--   0        0        0     5062 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/yfinance_view.py
--rw-r--r--   0        0        0      106 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/__init__.py
--rw-r--r--   0        0        0     4023 2023-06-07 00:09:56.321371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/disc_controller.py
--rw-r--r--   0        0        0     2804 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/wsj_model.py
--rw-r--r--   0        0        0     1320 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/wsj_view.py
--rw-r--r--   0        0        0    21045 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/etf_controller.py
--rw-r--r--   0        0        0      450 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/etf_helper.py
--rw-r--r--   0        0        0   188615 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/etfs.csv
--rw-r--r--   0        0        0     2608 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/financedatabase_model.py
--rw-r--r--   0        0        0     3864 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/financedatabase_view.py
--rw-r--r--   0        0        0     1417 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/fmp_model.py
--rw-r--r--   0        0        0     3152 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/fmp_view.py
--rw-r--r--   0        0        0     4172 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/stockanalysis_model.py
--rw-r--r--   0        0        0     3941 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/stockanalysis_view.py
--rw-r--r--   0        0        0    51458 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     6229 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/featflags_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/__init__.py
--rw-r--r--   0        0        0    58622 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/corporate_spot_rates.csv
--rw-r--r--   0        0        0     9217 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ecb_model.py
--rw-r--r--   0        0        0     7103 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ecb_view.py
--rw-r--r--   0        0        0     5811 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/econdb_model.py
--rw-r--r--   0        0        0     7831 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/econdb_view.py
--rw-r--r--   0        0        0    56238 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fixedincome_controller.py
--rw-r--r--   0        0        0    38003 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fred_model.py
--rw-r--r--   0        0        0    55506 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fred_view.py
--rw-r--r--   0        0        0   227110 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ice_bofa_indices.csv
--rw-r--r--   0        0        0    10963 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/oecd_model.py
--rw-r--r--   0        0        0     4004 2023-06-07 00:09:56.325371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/oecd_view.py
--rw-r--r--   0        0        0     2174 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/yfinance_model.py
--rw-r--r--   0        0        0     1702 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/anom_model.py
--rw-r--r--   0        0        0     2962 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/anom_view.py
--rw-r--r--   0        0        0     4629 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoarima_model.py
--rw-r--r--   0        0        0     3933 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoarima_view.py
--rw-r--r--   0        0        0     4658 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoces_model.py
--rw-r--r--   0        0        0     3970 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoces_view.py
--rw-r--r--   0        0        0     4694 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoets_model.py
--rw-r--r--   0        0        0     3972 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoets_view.py
--rw-r--r--   0        0        0     7567 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoselect_model.py
--rw-r--r--   0        0        0     3938 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoselect_view.py
--rw-r--r--   0        0        0     5874 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/brnn_model.py
--rw-r--r--   0        0        0     6577 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/brnn_view.py
--rw-r--r--   0        0        0     5562 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/expo_model.py
--rw-r--r--   0        0        0     5038 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/expo_view.py
--rw-r--r--   0        0        0     2053 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast.ipynb
--rw-r--r--   0        0        0   121975 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_controller.py
--rw-r--r--   0        0        0    15471 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_model.py
--rw-r--r--   0        0        0     9034 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_view.py
--rw-r--r--   0        0        0    47145 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/helpers.py
--rw-r--r--   0        0        0     3405 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/linregr_model.py
--rw-r--r--   0        0        0     4760 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/linregr_view.py
--rw-r--r--   0        0        0     5013 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/mstl_model.py
--rw-r--r--   0        0        0     3861 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/mstl_view.py
--rw-r--r--   0        0        0     5896 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nbeats_model.py
--rw-r--r--   0        0        0     6396 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nbeats_view.py
--rw-r--r--   0        0        0     7561 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nhits_model.py
--rw-r--r--   0        0        0     7952 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nhits_view.py
--rw-r--r--   0        0        0     3007 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/regr_model.py
--rw-r--r--   0        0        0     4521 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/regr_view.py
--rw-r--r--   0        0        0     5030 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rnn_model.py
--rw-r--r--   0        0        0     5533 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rnn_view.py
--rw-r--r--   0        0        0     4340 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rwd_model.py
--rw-r--r--   0        0        0     3643 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rwd_view.py
--rw-r--r--   0        0        0     4709 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/seasonalnaive_model.py
--rw-r--r--   0        0        0     3879 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/seasonalnaive_view.py
--rw-r--r--   0        0        0     5790 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tcn_model.py
--rw-r--r--   0        0        0     6289 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tcn_view.py
--rw-r--r--   0        0        0     7249 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tft_model.py
--rw-r--r--   0        0        0     6520 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tft_view.py
--rw-r--r--   0        0        0     4928 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/theta_model.py
--rw-r--r--   0        0        0     4379 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/theta_view.py
--rw-r--r--   0        0        0     6321 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/trans_model.py
--rw-r--r--   0        0        0     6765 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/trans_view.py
--rw-r--r--   0        0        0    12580 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/whisper_model.py
--rw-r--r--   0        0        0     2935 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/whisper_utils.py
--rw-r--r--   0        0        0      122 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/__init__.py
--rw-r--r--   0        0        0     5050 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/av_model.py
--rw-r--r--   0        0        0     1458 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/av_view.py
--rw-r--r--   0        0        0     3281 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/av_forex_currencies.csv
--rw-r--r--   0        0        0     7847 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/polygon_tickers.csv
--rw-r--r--   0        0        0   419838 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/yahoofinance_forex.json
--rw-r--r--   0        0        0    16492 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/forex_controller.py
--rw-r--r--   0        0        0     8201 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/forex_helper.py
--rw-r--r--   0        0        0      931 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/fxempire_model.py
--rw-r--r--   0        0        0     1471 2023-06-07 00:09:56.329371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/fxempire_view.py
--rw-r--r--   0        0        0    17162 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_controller.py
--rw-r--r--   0        0        0    22592 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_model.py
--rw-r--r--   0        0        0    12856 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_view.py
--rw-r--r--   0        0        0     2349 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/polygon_model.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0    26168 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0     1446 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/sdk_helpers.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/technical_analysis/__init__.py
--rw-r--r--   0        0        0    35136 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/databento_view.py
--rw-r--r--   0        0        0     9653 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/futures_controller.py
--rw-r--r--   0        0        0      358 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/futures_helper.py
--rw-r--r--   0        0        0      964 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/sdk_helper.py
--rw-r--r--   0        0        0     5669 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/yfinance_model.py
--rw-r--r--   0        0        0     8070 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/yfinance_view.py
--rw-r--r--   0        0        0    13050 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/helper_classes.py
--rw-r--r--   0        0        0    63148 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/helper_funcs.py
--rw-r--r--   0        0        0     3212 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/helpers_denomination.py
--rw-r--r--   0        0        0     9743 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/intro.json
--rw-r--r--   0        0        0    45225 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_controller.py
--rw-r--r--   0        0        0    84278 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_model.py
--rw-r--r--   0        0        0     1148 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_view.py
--rw-r--r--   0        0        0    11456 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/loggers.py
--rw-r--r--   0        0        0     1701 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/menu.py
--rw-r--r--   0        0        0    23784 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.csv
--rw-r--r--   0        0        0    29952 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.json
--rw-r--r--   0        0        0     6403 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.csv
--rw-r--r--   0        0        0     8797 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.json
--rw-r--r--   0        0        0    11455 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/generate_documentation_commands.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/custom/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/economy/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
--rw-r--r--   0        0        0     8528 2023-06-07 00:09:56.333371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/futures/futures.csv
--rw-r--r--   0        0        0    60375 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/i18n/en.yml
--rw-r--r--   0        0        0     5831 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
--rw-r--r--   0        0        0     3868 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD
--rw-r--r--   0        0        0      101 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
--rw-r--r--   0        0        0       66 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt.openbb
--rw-r--r--   0        0        0       87 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_covid.openbb
--rw-r--r--   0        0        0      164 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_oss.openbb
--rw-r--r--   0        0        0      209 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_realestate.openbb
--rw-r--r--   0        0        0      936 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
--rw-r--r--   0        0        0     1039 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_dd.openbb
--rw-r--r--   0        0        0     1319 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_defi.openbb
--rw-r--r--   0        0        0      582 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_discovery.openbb
--rw-r--r--   0        0        0      195 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_nft.openbb
--rw-r--r--   0        0        0     1287 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_onchain.openbb
--rw-r--r--   0        0        0     1606 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_overview.openbb
--rw-r--r--   0        0        0      604 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_qa.openbb
--rw-r--r--   0        0        0      850 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_ta.openbb
--rw-r--r--   0        0        0      165 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_tools.openbb
--rw-r--r--   0        0        0      132 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards.openbb
--rw-r--r--   0        0        0     1440 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics.openbb
--rw-r--r--   0        0        0     2436 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
--rw-r--r--   0        0        0      274 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_qa.openbb
--rw-r--r--   0        0        0       41 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ca.openbb
--rw-r--r--   0        0        0      265 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_disc.openbb
--rw-r--r--   0        0        0      227 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
--rw-r--r--   0        0        0      890 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ta.openbb
--rw-r--r--   0        0        0     2301 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
--rw-r--r--   0        0        0      521 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
--rw-r--r--   0        0        0      449 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex.openbb
--rw-r--r--   0        0        0      791 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_oanda.openbb
--rw-r--r--   0        0        0      654 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_qa.openbb
--rw-r--r--   0        0        0      636 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_ta.openbb
--rw-r--r--   0        0        0      184 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
--rw-r--r--   0        0        0       16 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/keys/test_keys.openbb
--rw-r--r--   0        0        0      277 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/mutual_funds/test_mutual_fund.openbb
--rw-r--r--   0        0        0      109 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_params.openbb
--rw-r--r--   0        0        0     1967 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po.openbb
--rw-r--r--   0        0        0     1850 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
--rw-r--r--   0        0        0      509 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports.openbb
--rw-r--r--   0        0        0      272 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ba.openbb
--rw-r--r--   0        0        0     1524 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_bt.openbb
--rw-r--r--   0        0        0      635 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ca.openbb
--rw-r--r--   0        0        0      282 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_disc.openbb
--rw-r--r--   0        0        0      177 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_dps.openbb
--rw-r--r--   0        0        0     1741 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_fa.openbb
--rw-r--r--   0        0        0       21 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_forecast.openbb
--rw-r--r--   0        0        0      481 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_gov.openbb
--rw-r--r--   0        0        0      154 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_hedge.openbb
--rw-r--r--   0        0        0      236 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_insider.openbb
--rw-r--r--   0        0        0      361 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_options.openbb
--rw-r--r--   0        0        0      671 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_qa.openbb
--rw-r--r--   0        0        0       47 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_res.openbb
--rw-r--r--   0        0        0      163 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_screener.openbb
--rw-r--r--   0        0        0      735 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
--rw-r--r--   0        0        0      768 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ta.openbb
--rw-r--r--   0        0        0      102 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_tradinghours.openbb
--rw-r--r--   0        0        0       46 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/terminal/test_news.openbb
--rw-r--r--   0        0        0     1065 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/models/hub_credentials.json
--rw-r--r--   0        0        0      380 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/models/local_credentials.json
--rw-r--r--   0        0        0    17970 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
--rw-r--r--   0        0        0    29757 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
--rw-r--r--   0        0        0    33733 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/parameters_template.xlsx
--rw-r--r--   0        0        0      310 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/routines/routine_example.openbb
--rw-r--r--   0        0        0    21793 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/sources/openbb_default.json
--rw-r--r--   0        0        0     2332 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
--rw-r--r--   0        0        0     2354 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
--rw-r--r--   0        0        0     2341 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
--rw-r--r--   0        0        0     2316 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
--rw-r--r--   0        0        0     2316 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
--rw-r--r--   0        0        0     2346 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
--rw-r--r--   0        0        0     2336 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
--rw-r--r--   0        0        0     2346 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
--rw-r--r--   0        0        0     2307 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
--rw-r--r--   0        0        0     2309 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
--rw-r--r--   0        0        0     2329 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
--rw-r--r--   0        0        0     2353 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
--rw-r--r--   0        0        0     2360 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
--rw-r--r--   0        0        0     2320 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
--rw-r--r--   0        0        0     2344 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
--rw-r--r--   0        0        0     2315 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
--rw-r--r--   0        0        0     2346 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
--rw-r--r--   0        0        0     2376 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
--rw-r--r--   0        0        0     2326 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Health.ini
--rw-r--r--   0        0        0     2307 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
--rw-r--r--   0        0        0     2320 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
--rw-r--r--   0        0        0     2324 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
--rw-r--r--   0        0        0     2334 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
--rw-r--r--   0        0        0     2324 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
--rw-r--r--   0        0        0     2313 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
--rw-r--r--   0        0        0     2341 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
--rw-r--r--   0        0        0     2296 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
--rw-r--r--   0        0        0     2367 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
--rw-r--r--   0        0        0     2342 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
--rw-r--r--   0        0        0     2361 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
--rw-r--r--   0        0        0     2351 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
--rw-r--r--   0        0        0     2336 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
--rw-r--r--   0        0        0     2322 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
--rw-r--r--   0        0        0     2310 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
--rw-r--r--   0        0        0     2326 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
--rw-r--r--   0        0        0     2341 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
--rw-r--r--   0        0        0     2299 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
--rw-r--r--   0        0        0     2316 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
--rw-r--r--   0        0        0     2342 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
--rw-r--r--   0        0        0     2381 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
--rw-r--r--   0        0        0     2314 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
--rw-r--r--   0        0        0    34473 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/template.ini
--rw-r--r--   0        0        0    34519 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/whales.ini
--rwxr-xr-x   0        0        0      282 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
--rw-r--r--   0        0        0    21940 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
--rwxr-xr-x   0        0        0      315 2023-06-07 00:09:56.337371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
--rwxr-xr-x   0        0        0      464 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
--rw-r--r--   0        0        0      413 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
--rwxr-xr-x   0        0        0      184 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
--rwxr-xr-x   0        0        0      364 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
--rw-r--r--   0        0        0      326 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
--rw-r--r--   0        0        0      193 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
--rw-r--r--   0        0        0      241 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
--rwxr-xr-x   0        0        0      335 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
--rw-r--r--   0        0        0      286 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
--rwxr-xr-x   0        0        0      167 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
--rw-r--r--   0        0        0      221 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
--rwxr-xr-x   0        0        0      255 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
--rwxr-xr-x   0        0        0      518 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
--rw-r--r--   0        0        0      302 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
--rwxr-xr-x   0        0        0      279 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
--rw-r--r--   0        0        0      316 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
--rw-r--r--   0        0        0      349 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
--rwxr-xr-x   0        0        0      295 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
--rwxr-xr-x   0        0        0      274 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
--rwxr-xr-x   0        0        0      328 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
--rwxr-xr-x   0        0        0      301 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
--rwxr-xr-x   0        0        0      212 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
--rwxr-xr-x   0        0        0      295 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
--rw-r--r--   0        0        0      337 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
--rw-r--r--   0        0        0      280 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
--rw-r--r--   0        0        0      246 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
--rw-r--r--   0        0        0      360 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
--rwxr-xr-x   0        0        0      222 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
--rwxr-xr-x   0        0        0      260 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
--rwxr-xr-x   0        0        0      197 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
--rwxr-xr-x   0        0        0      211 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
--rwxr-xr-x   0        0        0      201 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
--rwxr-xr-x   0        0        0      203 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
--rwxr-xr-x   0        0        0      179 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
--rwxr-xr-x   0        0        0      185 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
--rwxr-xr-x   0        0        0      187 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
--rwxr-xr-x   0        0        0      189 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
--rwxr-xr-x   0        0        0      189 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
--rwxr-xr-x   0        0        0      187 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
--rwxr-xr-x   0        0        0      185 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
--rwxr-xr-x   0        0        0      276 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
--rwxr-xr-x   0        0        0      272 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
--rwxr-xr-x   0        0        0      299 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
--rwxr-xr-x   0        0        0      293 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
--rwxr-xr-x   0        0        0      286 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
--rw-r--r--   0        0        0      209 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
--rwxr-xr-x   0        0        0      272 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
--rwxr-xr-x   0        0        0      675 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
--rwxr-xr-x   0        0        0      315 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
--rw-r--r--   0        0        0   358460 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
--rw-r--r--   0        0        0      972 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
--rw-r--r--   0        0        0     2086 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
--rw-r--r--   0        0        0     2750 2023-06-07 00:09:56.341371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0      203 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
--rw-r--r--   0        0        0      970 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
--rw-r--r--   0        0        0      182 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
--rw-r--r--   0        0        0     2035 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.mplstyle
--rw-r--r--   0        0        0    24193 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0      202 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
--rw-r--r--   0        0        0     2607 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0      186 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
--rw-r--r--   0        0        0      144 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/__init__.py
--rw-r--r--   0        0        0    81373 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_fund_ID.csv
--rw-r--r--   0        0        0      834 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_model.py
--rw-r--r--   0        0        0     3941 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_view.py
--rw-r--r--   0        0        0     6535 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mstarpy_model.py
--rw-r--r--   0        0        0     7883 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mstarpy_view.py
--rw-r--r--   0        0        0    15141 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mutual_fund_controller.py
--rw-r--r--   0        0        0     6040 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mutual_funds_utils.py
--rw-r--r--   0        0        0    50383 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/parent_classes.py
--rw-r--r--   0        0        0       61 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/__init__.py
--rw-r--r--   0        0        0    15080 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/allocation_model.py
--rw-r--r--   0        0        0    12944 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/attribution_model.py
--rw-r--r--   0        0        0      417 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/__init__.py
--rw-r--r--   0        0        0     3214 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/bro_controller.py
--rw-r--r--   0        0        0     1121 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/brokers_helpers.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/__init__.py
--rw-r--r--   0        0        0     8211 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
--rw-r--r--   0        0        0     9561 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
--rw-r--r--   0        0        0     4495 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
--rw-r--r--   0        0        0     4666 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/__init__.py
--rw-r--r--   0        0        0    12789 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
--rw-r--r--   0        0        0    15571 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
--rw-r--r--   0        0        0    15670 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
--rw-r--r--   0        0        0     3894 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
--rw-r--r--   0        0        0     3002 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
--rw-r--r--   0        0        0     2482 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
--rw-r--r--   0        0        0    30861 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/metrics_model.py
--rw-r--r--   0        0        0    54979 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_controller.py
--rw-r--r--   0        0        0    39188 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_engine.py
--rw-r--r--   0        0        0     9643 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_helper.py
--rw-r--r--   0        0        0    60205 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_model.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/__init__.py
--rw-r--r--   0        0        0     5255 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
--rw-r--r--   0        0        0     2106 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
--rw-r--r--   0        0        0   120571 2023-06-07 00:09:56.345371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
--rw-r--r--   0        0        0   155050 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
--rw-r--r--   0        0        0     2773 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
--rw-r--r--   0        0        0    13116 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
--rw-r--r--   0        0        0     5974 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
--rw-r--r--   0        0        0     5346 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
--rw-r--r--   0        0        0     4427 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
--rw-r--r--   0        0        0   138034 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
--rw-r--r--   0        0        0     8587 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
--rw-r--r--   0        0        0   103568 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_model.py
--rw-r--r--   0        0        0    24186 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_view.py
--rw-r--r--   0        0        0    11390 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/statics.py
--rw-r--r--   0        0        0    12009 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
--rw-r--r--   0        0        0    54951 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_view.py
--rw-r--r--   0        0        0     8433 2023-06-07 00:09:56.349371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/statics.py
--rw-r--r--   0        0        0  1028287 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
--rw-r--r--   0        0        0     2839 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/__init__.py
--rw-r--r--   0        0        0      443 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/data/crypto_tickers.csv
--rw-r--r--   0        0        0      437 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/data/etf_tickers.csv
--rw-r--r--   0        0        0      222 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/data/stocks_tickers.csv
--rw-r--r--   0        0        0     9706 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/reports_controller.py
--rw-r--r--   0        0        0    12310 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/reports_model.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.353371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/stored/.gitkeep
--rw-r--r--   0        0        0  1076317 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
--rw-r--r--   0        0        0     5214 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/OpenBB_reports_logo.png
--rw-r--r--   0        0        0    32656 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/crypto.ipynb
--rw-r--r--   0        0        0    25803 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/economy.ipynb
--rw-r--r--   0        0        0    40287 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/equity.ipynb
--rw-r--r--   0        0        0    13582 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/etf.ipynb
--rw-r--r--   0        0        0     2782 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/floppy-disc.png
--rw-r--r--   0        0        0     8567 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/forecast.ipynb
--rw-r--r--   0        0        0    17778 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/forex.ipynb
--rw-r--r--   0        0        0    14922 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/portfolio.ipynb
--rw-r--r--   0        0        0    11247 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widget_helpers.py
--rw-r--r--   0        0        0      205 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/card.j2
--rw-r--r--   0        0        0     3556 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/report.css
--rw-r--r--   0        0        0      474 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/report.j2
--rw-r--r--   0        0        0      119 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/row.j2
--rw-r--r--   0        0        0      896 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/style.css
--rw-r--r--   0        0        0     9967 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/rich_config.py
--rw-r--r--   0        0        0    20276 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/routine_functions.py
--rw-r--r--   0        0        0    31224 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/sdk.py
--rw-r--r--   0        0        0    20375 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/settings_controller.py
--rw-r--r--   0        0        0     7105 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/sources_controller.py
--rw-r--r--   0        0        0      357 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/__init__.py
--rw-r--r--   0        0        0    10448 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_controller.py
--rw-r--r--   0        0        0     8126 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_model.py
--rw-r--r--   0        0        0     9046 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/__init__.py
--rw-r--r--   0        0        0    29872 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
--rw-r--r--   0        0        0     3541 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3761 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
--rw-r--r--   0        0        0     1931 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/cboe_model.py
--rw-r--r--   0        0        0      969 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/cboe_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/__init__.py
--rw-r--r--   0        0        0    37621 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/ca_controller.py
--rw-r--r--   0        0        0     4871 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
--rw-r--r--   0        0        0     5859 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1328 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
--rw-r--r--   0        0        0     2738 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
--rw-r--r--   0        0        0     1539 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
--rw-r--r--   0        0        0    12451 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     5957 2023-06-07 00:09:56.361371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     1690 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/polygon_model.py
--rw-r--r--   0        0        0     1379 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
--rw-r--r--   0        0        0     8073 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    10164 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/__init__.py
--rw-r--r--   0        0        0    20377 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
--rw-r--r--   0        0        0     9982 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
--rw-r--r--   0        0        0     7203 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
--rw-r--r--   0        0        0     1093 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
--rw-r--r--   0        0        0     1200 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
--rw-r--r--   0        0        0     1387 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
--rw-r--r--   0        0        0     4816 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
--rw-r--r--   0        0        0     6836 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
--rw-r--r--   0        0        0     3477 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
--rw-r--r--   0        0        0     1882 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
--rw-r--r--   0        0        0     1385 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
--rw-r--r--   0        0        0     5053 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
--rw-r--r--   0        0        0     9997 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
--rw-r--r--   0        0        0     1166 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
--rw-r--r--   0        0        0     3769 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
--rw-r--r--   0        0        0      668 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
--rw-r--r--   0        0        0     1271 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
--rw-r--r--   0        0        0     4421 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/databento_model.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/__init__.py
--rw-r--r--   0        0        0     4169 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/ark_model.py
--rw-r--r--   0        0        0     2589 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/ark_view.py
--rw-r--r--   0        0        0    29463 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/disc_controller.py
--rw-r--r--   0        0        0      483 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/disc_helpers.py
--rw-r--r--   0        0        0     2696 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fidelity_model.py
--rw-r--r--   0        0        0     2610 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fidelity_view.py
--rw-r--r--   0        0        0     4164 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finnhub_model.py
--rw-r--r--   0        0        0     2510 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finnhub_view.py
--rw-r--r--   0        0        0     1731 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finviz_model.py
--rw-r--r--   0        0        0     3084 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finviz_view.py
--rw-r--r--   0        0        0     2562 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fmp_view.py
--rw-r--r--   0        0        0     3051 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/nasdaq_model.py
--rw-r--r--   0        0        0     3406 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/nasdaq_view.py
--rw-r--r--   0        0        0     5934 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/seeking_alpha_model.py
--rw-r--r--   0        0        0     3485 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/seeking_alpha_view.py
--rw-r--r--   0        0        0     1120 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/shortinterest_model.py
--rw-r--r--   0        0        0     2566 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/shortinterest_view.py
--rw-r--r--   0        0        0     4113 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/yahoofinance_model.py
--rw-r--r--   0        0        0     5871 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/yahoofinance_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/__init__.py
--rw-r--r--   0        0        0    24126 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/av_model.py
--rw-r--r--   0        0        0    14922 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/av_view.py
--rw-r--r--   0        0        0     8170 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
--rw-r--r--   0        0        0     7775 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
--rw-r--r--   0        0        0     1833 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
--rw-r--r--   0        0        0     2347 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
--rw-r--r--   0        0        0    14744 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
--rw-r--r--   0        0        0     4279 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
--rw-r--r--   0        0        0    44494 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
--rw-r--r--   0        0        0     1925 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
--rw-r--r--   0        0        0     1205 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
--rw-r--r--   0        0        0     2396 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
--rw-r--r--   0        0        0     4904 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
--rw-r--r--   0        0        0    81997 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
--rw-r--r--   0        0        0      266 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
--rw-r--r--   0        0        0     1389 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
--rw-r--r--   0        0        0     3518 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
--rw-r--r--   0        0        0     3478 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
--rw-r--r--   0        0        0     2484 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
--rw-r--r--   0        0        0    22344 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
--rw-r--r--   0        0        0    23771 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
--rw-r--r--   0        0        0     6417 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
--rw-r--r--   0        0        0    11893 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
--rw-r--r--   0        0        0     1350 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
--rw-r--r--   0        0        0     2654 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/nasdaq_model.py
--rw-r--r--   0        0        0     1862 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/nasdaq_view.py
--rw-r--r--   0        0        0     5391 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
--rw-r--r--   0        0        0     4360 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
--rw-r--r--   0        0        0     8546 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
--rw-r--r--   0        0        0    11162 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
--rw-r--r--   0        0        0     2059 2023-06-07 00:09:56.365371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
--rw-r--r--   0        0        0    11817 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
--rw-r--r--   0        0        0    14162 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/__init__.py
--rw-r--r--   0        0        0    18461 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/gov_controller.py
--rw-r--r--   0        0        0    15719 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/quiverquant_model.py
--rw-r--r--   0        0        0    21428 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/quiverquant_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/__init__.py
--rw-r--r--   0        0        0     2062 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/businessinsider_model.py
--rw-r--r--   0        0        0     5102 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/businessinsider_view.py
--rw-r--r--   0        0        0     1125 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/finviz_model.py
--rw-r--r--   0        0        0     1171 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/finviz_view.py
--rw-r--r--   0        0        0    32744 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/insider_controller.py
--rw-r--r--   0        0        0    87495 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/openinsider_model.py
--rw-r--r--   0        0        0     7695 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/openinsider_view.py
--rw-r--r--   0        0        0     4909 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/sdk_helper.py
--rw-r--r--   0        0        0    76085 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/mappings/Mic_Codes.csv
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/alphaquery_model.py
--rw-r--r--   0        0        0     1713 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/alphaquery_view.py
--rw-r--r--   0        0        0     1161 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/barchart_model.py
--rw-r--r--   0        0        0     1137 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/barchart_view.py
--rw-r--r--   0        0        0     1526 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/calculator_model.py
--rw-r--r--   0        0        0     2416 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/calculator_view.py
--rw-r--r--   0        0        0     2777 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/chartexchange_model.py
--rw-r--r--   0        0        0     3271 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/chartexchange_view.py
--rw-r--r--   0        0        0     2433 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/fdscanner_model.py
--rw-r--r--   0        0        0     1672 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/fdscanner_view.py
--rw-r--r--   0        0        0    21092 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_controller.py
--rw-r--r--   0        0        0     9884 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_model.py
--rw-r--r--   0        0        0     3968 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_view.py
--rw-r--r--   0        0        0    10111 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/intrinio_model.py
--rw-r--r--   0        0        0     6390 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/intrinio_view.py
--rw-r--r--   0        0        0     7070 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/nasdaq_model.py
--rw-r--r--   0        0        0    17467 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/op_helpers.py
--rw-r--r--   0        0        0    51114 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_controller.py
--rw-r--r--   0        0        0     9034 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_sdk_helper.py
--rw-r--r--   0        0        0    14494 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_view.py
--rw-r--r--   0        0        0     8410 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/tradier_model.py
--rw-r--r--   0        0        0     2903 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/tradier_view.py
--rw-r--r--   0        0        0     7647 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/yfinance_model.py
--rw-r--r--   0        0        0    11535 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/yfinance_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/__init__.py
--rw-r--r--   0        0        0     2260 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/beta_model.py
--rw-r--r--   0        0        0     2798 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/beta_view.py
--rw-r--r--   0        0        0     3187 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/factors_model.py
--rw-r--r--   0        0        0      687 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/factors_view.py
--rw-r--r--   0        0        0    38741 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
--rw-r--r--   0        0        0      447 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/qa_model.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/research/__init__.py
--rw-r--r--   0        0        0     6218 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/research/res_controller.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/__init__.py
--rw-r--r--   0        0        0    46671 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/finviz_model.py
--rw-r--r--   0        0        0     7192 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/finviz_view.py
--rw-r--r--   0        0        0    21493 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_controller.py
--rw-r--r--   0        0        0      944 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_helper.py
--rw-r--r--   0        0        0     2562 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_view.py
--rw-r--r--   0        0        0    27722 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stock_statics.py
--rw-r--r--   0        0        0    28108 2023-06-07 00:09:56.369371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_controller.py
--rw-r--r--   0        0        0    35085 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_helper.py
--rw-r--r--   0        0        0    11340 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_model.py
--rw-r--r--   0        0        0     1559 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/__init__.py
--rw-r--r--   0        0        0     1004 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/finbrain_model.py
--rw-r--r--   0        0        0      644 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/finbrain_view.py
--rw-r--r--   0        0        0     1532 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/rsp_model.py
--rw-r--r--   0        0        0     2386 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/rsp_view.py
--rw-r--r--   0        0        0    65324 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/ta_controller.py
--rw-r--r--   0        0        0     3260 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/tradingview_model.py
--rw-r--r--   0        0        0     1985 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/tradingview_view.py
--rw-r--r--   0        0        0      334 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/README.md
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/__init__.py
--rw-r--r--   0        0        0     5328 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/bursa_model.py
--rw-r--r--   0        0        0     2202 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/bursa_view.py
--rw-r--r--   0        0        0        0 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/data/__init__.py
--rw-r--r--   0        0        0    28098 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
--rw-r--r--   0        0        0     1466 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
--rw-r--r--   0        0        0     1378 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
--rw-r--r--   0        0        0    10137 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
--rw-r--r--   0        0        0      614 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
--rw-r--r--   0        0        0    42676 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/terminal_controller.py
--rw-r--r--   0        0        0    14590 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/terminal_helper.py
--rw-r--r--   0        0        0     3848 2023-06-07 00:09:56.373371 openbb_nightly-3.0.1.dev20230607/openbb_terminal/thought_of_the_day.py
--rw-r--r--   0        0        0     5737 2023-06-07 00:09:58.205360 openbb_nightly-3.0.1.dev20230607/pyproject.toml
--rw-r--r--   0        0        0     1145 2023-06-07 00:09:56.377371 openbb_nightly-3.0.1.dev20230607/terminal.py
--rw-r--r--   0        0        0     2285 2023-06-07 00:09:58.209360 openbb_nightly-3.0.1.dev20230607/website/pypi.md
--rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 openbb_nightly-3.0.1.dev20230607/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-08 00:09:53.040142 openbb_nightly-3.0.1.dev20230608/LICENSE
+-rw-r--r--   0        0        0      243 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/__init__.py
+-rw-r--r--   0        0        0    22105 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/account_controller.py
+-rw-r--r--   0        0        0     1769 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/account_view.py
+-rw-r--r--   0        0        0      419 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/show_prompt.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/__init__.py
+-rw-r--r--   0        0        0     3131 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/alt_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/countries.txt
+-rw-r--r--   0        0        0     9347 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_controller.py
+-rw-r--r--   0        0        0     5388 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_model.py
+-rw-r--r--   0        0        0     8586 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_view.py
+-rw-r--r--   0        0        0     1070 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/hackernews_model.py
+-rw-r--r--   0        0        0     1087 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/hackernews_view.py
+-rw-r--r--   0        0        0     6752 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/github_model.py
+-rw-r--r--   0        0        0     3968 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/github_view.py
+-rw-r--r--   0        0        0     8656 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/oss_controller.py
+-rw-r--r--   0        0        0     4437 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/runa_model.py
+-rw-r--r--   0        0        0     4018 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/runa_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.228145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/__init__.py
+-rw-r--r--   0        0        0     9030 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/landRegistry_model.py
+-rw-r--r--   0        0        0     3309 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/landRegistry_view.py
+-rw-r--r--   0        0        0     8108 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/realestate_controller.py
+-rw-r--r--   0        0        0     2865 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/base_helpers.py
+-rw-r--r--   0        0        0       93 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0     1198 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     4401 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1335 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     1861 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3329 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/google_model.py
+-rw-r--r--   0        0        0     7118 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/google_view.py
+-rw-r--r--   0        0        0     5524 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_helpers.py
+-rw-r--r--   0        0        0    18297 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_model.py
+-rw-r--r--   0        0        0    10170 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_view.py
+-rw-r--r--   0        0        0     3239 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/stocktwits_model.py
+-rw-r--r--   0        0        0     2898 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/stocktwits_view.py
+-rw-r--r--   0        0        0     6160 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/twitter_model.py
+-rw-r--r--   0        0        0     5870 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/twitter_view.py
+-rw-r--r--   0        0        0     4956 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/biztoc_model.py
+-rw-r--r--   0        0        0     2341 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/biztoc_view.py
+-rw-r--r--   0        0        0     4142 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/common_model.py
+-rw-r--r--   0        0        0     3634 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/feedparser_model.py
+-rw-r--r--   0        0        0     1442 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/feedparser_view.py
+-rw-r--r--   0        0        0     1435 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/news_sdk_helper.py
+-rw-r--r--   0        0        0     2639 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/newsapi_model.py
+-rw-r--r--   0        0        0     1465 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/newsapi_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    19923 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0    32308 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/qa_view.py
+-rw-r--r--   0        0        0     3226 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/rolling_model.py
+-rw-r--r--   0        0        0    10790 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/rolling_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     2993 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/custom_indicators_model.py
+-rw-r--r--   0        0        0     4272 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/custom_indicators_view.py
+-rw-r--r--   0        0        0     6427 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/momentum_model.py
+-rw-r--r--   0        0        0    12480 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/momentum_view.py
+-rw-r--r--   0        0        0     4179 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/overlap_model.py
+-rw-r--r--   0        0        0     4430 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/overlap_view.py
+-rw-r--r--   0        0        0     1453 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/ta_helpers.py
+-rw-r--r--   0        0        0     1819 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/trend_indicators_model.py
+-rw-r--r--   0        0        0     2621 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/trend_indicators_view.py
+-rw-r--r--   0        0        0    19962 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volatility_model.py
+-rw-r--r--   0        0        0    10005 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volatility_view.py
+-rw-r--r--   0        0        0     2614 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volume_model.py
+-rw-r--r--   0        0        0     3806 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volume_view.py
+-rw-r--r--   0        0        0     7577 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/ultima_newsmonitor_model.py
+-rw-r--r--   0        0        0     4870 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/ultima_newsmonitor_view.py
+-rw-r--r--   0        0        0     2634 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/config_terminal.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/__init__.py
+-rw-r--r--   0        0        0     9829 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/completer/choices.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/config/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/config/paths.py
+-rw-r--r--   0        0        0     2650 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/config/paths_helper.py
+-rw-r--r--   0        0        0     9830 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/README.md
+-rw-r--r--   0        0        0     2081 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/controllers.json
+-rw-r--r--   0        0        0    23202 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/integration_controller.py
+-rw-r--r--   0        0        0    20084 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/integration_test_coverage.py
+-rw-r--r--   0        0        0     3389 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/__init__.py
+-rw-r--r--   0        0        0     3904 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/log_sender.py
+-rw-r--r--   0        0        0     3744 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/logging_clock.py
+-rw-r--r--   0        0        0     3495 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/s3_sender.py
+-rw-r--r--   0        0        0      166 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/constants.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/common.py
+-rw-r--r--   0        0        0      631 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/custom_logger.py
+-rw-r--r--   0        0        0      979 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/directories.py
+-rw-r--r--   0        0        0      841 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/expired_files.py
+-rw-r--r--   0        0        0     5239 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     6058 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4200 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/settings.py
+-rw-r--r--   0        0        0     1818 2023-06-08 00:09:53.232145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/settings_logger.py
+-rw-r--r--   0        0        0      396 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/user_logger.py
+-rw-r--r--   0        0        0      627 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/base_model.py
+-rw-r--r--   0        0        0      818 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/credentials_model.py
+-rw-r--r--   0        0        0     3708 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/preferences_model.py
+-rw-r--r--   0        0        0     2041 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/profile_model.py
+-rw-r--r--   0        0        0     1230 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/sources_model.py
+-rw-r--r--   0        0        0     2922 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/system_model.py
+-rw-r--r--   0        0        0      634 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/user_model.py
+-rw-r--r--   0        0        0      200 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/__init__.py
+-rw-r--r--   0        0        0   418780 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/assets/Terminal_icon.png
+-rw-r--r--   0        0        0    14244 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/backend.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/config/__init__.py
+-rw-r--r--   0        0        0     7156 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/config/openbb_styles.py
+-rw-r--r--   0        0        0     3132 2023-06-08 00:09:53.236145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/no_import.py
+-rw-r--r--   0        0        0  4433681 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly.html
+-rw-r--r--   0        0        0    63492 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_helper.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     6724 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/base.py
+-rw-r--r--   0        0        0    11370 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0     8004 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    18320 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3339 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5683 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6844 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3429 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    20601 2023-06-08 00:09:53.260145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0   711999 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/table.html
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/scripts/__init__.py
+-rw-r--r--   0        0        0     7775 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/scripts/sdk_audit.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/__init__.py
+-rw-r--r--   0        0        0      450 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py
+-rw-r--r--   0        0        0    24817 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py
+-rw-r--r--   0        0        0     1513 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py
+-rw-r--r--   0        0        0     2365 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py
+-rw-r--r--   0        0        0     5128 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py
+-rw-r--r--   0        0        0    18025 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py
+-rw-r--r--   0        0        0      761 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/__init__.py
+-rw-r--r--   0        0        0     4308 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/alt_sdk_model.py
+-rw-r--r--   0        0        0    44505 2023-06-08 00:09:53.264145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/crypto_sdk_model.py
+-rw-r--r--   0        0        0     4889 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/econometrics_sdk_model.py
+-rw-r--r--   0        0        0     7830 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/economy_sdk_model.py
+-rw-r--r--   0        0        0     2496 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/etf_sdk_model.py
+-rw-r--r--   0        0        0     3515 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py
+-rw-r--r--   0        0        0     8550 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/forecast_sdk_model.py
+-rw-r--r--   0        0        0     4386 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/forex_sdk_model.py
+-rw-r--r--   0        0        0     1530 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/funds_sdk_model.py
+-rw-r--r--   0        0        0     1067 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/futures_sdk_model.py
+-rw-r--r--   0        0        0     3725 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/keys_sdk_model.py
+-rw-r--r--   0        0        0    10046 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/portfolio_sdk_model.py
+-rw-r--r--   0        0        0     4603 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/qa_sdk_model.py
+-rw-r--r--   0        0        0    31836 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/stocks_sdk_model.py
+-rw-r--r--   0        0        0     7229 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/ta_sdk_model.py
+-rw-r--r--   0        0        0    11588 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/sdk_helpers.py
+-rw-r--r--   0        0        0    19897 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/sdk_init.py
+-rw-r--r--   0        0        0    44090 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map.csv
+-rw-r--r--   0        0        0     2801 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map_forecasting.csv
+-rw-r--r--   0        0        0     1301 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map_optimization.csv
+-rw-r--r--   0        0        0     6971 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trailmap.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/banner.txt
+-rw-r--r--   0        0        0      602 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/constants.py
+-rw-r--r--   0        0        0     1000 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/current_system.py
+-rw-r--r--   0        0        0     4095 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/current_user.py
+-rw-r--r--   0        0        0     1400 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/env_handler.py
+-rw-r--r--   0        0        0    22314 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/hub_model.py
+-rw-r--r--   0        0        0     6162 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/local_model.py
+-rw-r--r--   0        0        0     6205 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/routines_handler.py
+-rw-r--r--   0        0        0     3672 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/sdk_session.py
+-rw-r--r--   0        0        0     3193 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/session_controller.py
+-rw-r--r--   0        0        0     6308 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/session_model.py
+-rw-r--r--   0        0        0     2834 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/sources_handler.py
+-rw-r--r--   0        0        0     1677 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/utils.py
+-rw-r--r--   0        0        0     3011 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sources/utils.py
+-rw-r--r--   0        0        0      199 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/README.md
+-rw-r--r--   0        0        0       84 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/__init__.py
+-rw-r--r--   0        0        0     5303 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/coinbase_helpers.py
+-rw-r--r--   0        0        0     2147 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/coinpaprika_helpers.py
+-rw-r--r--   0        0        0    19295 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_controller.py
+-rw-r--r--   0        0        0     4481 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_models.py
+-rw-r--r--   0        0        0     1785 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_views.py
+-rw-r--r--   0        0        0    30340 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py
+-rw-r--r--   0        0        0      949 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/README.md
+-rw-r--r--   0        0        0     7341 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/binance_gecko_map.json
+-rw-r--r--   0        0        0     2436 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json
+-rw-r--r--   0        0        0     4813 2023-06-08 00:09:53.268145 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coingecko_categories.json
+-rw-r--r--   0        0        0   954385 2023-06-08 00:09:53.272146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coingecko_coins.json
+-rw-r--r--   0        0        0  2245016 2023-06-08 00:09:53.280146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json
+-rw-r--r--   0        0        0    31307 2023-06-08 00:09:53.280146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/defillama_dapps.json
+-rw-r--r--   0        0        0   107203 2023-06-08 00:09:53.280146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/erc20_coins.json
+-rw-r--r--   0        0        0     7255 2023-06-08 00:09:53.280146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/finbrain_coins.json
+-rw-r--r--   0        0        0   222978 2023-06-08 00:09:53.280146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/santiment_slugs.json
+-rw-r--r--   0        0        0   300253 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json
+-rw-r--r--   0        0        0     4951 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/dataframe_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/__init__.py
+-rw-r--r--   0        0        0     4537 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/coindix_model.py
+-rw-r--r--   0        0        0     2720 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/coindix_view.py
+-rw-r--r--   0        0        0     2629 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py
+-rw-r--r--   0        0        0     2127 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py
+-rw-r--r--   0        0        0    31284 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/defi_controller.py
+-rw-r--r--   0        0        0     8918 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/graph_model.py
+-rw-r--r--   0        0        0     7165 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/graph_view.py
+-rw-r--r--   0        0        0     5005 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/llama_model.py
+-rw-r--r--   0        0        0     5827 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/llama_view.py
+-rw-r--r--   0        0        0     1808 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/smartstake_model.py
+-rw-r--r--   0        0        0     3110 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/smartstake_view.py
+-rw-r--r--   0        0        0     2882 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/substack_model.py
+-rw-r--r--   0        0        0     1090 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/substack_view.py
+-rw-r--r--   0        0        0     1947 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terraengineer_model.py
+-rw-r--r--   0        0        0     2699 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terraengineer_view.py
+-rw-r--r--   0        0        0     9734 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py
+-rw-r--r--   0        0        0     8022 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/__init__.py
+-rw-r--r--   0        0        0     2317 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py
+-rw-r--r--   0        0        0     1620 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py
+-rw-r--r--   0        0        0     2116 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py
+-rw-r--r--   0        0        0     1936 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py
+-rw-r--r--   0        0        0    10255 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/dappradar_model.py
+-rw-r--r--   0        0        0     8161 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/dappradar_view.py
+-rw-r--r--   0        0        0    24664 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    10833 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py
+-rw-r--r--   0        0        0     6352 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py
+-rw-r--r--   0        0        0     1095 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/__init__.py
+-rw-r--r--   0        0        0     7483 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/binance_model.py
+-rw-r--r--   0        0        0     3009 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/binance_view.py
+-rw-r--r--   0        0        0     3188 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py
+-rw-r--r--   0        0        0     2840 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py
+-rw-r--r--   0        0        0     6439 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py
+-rw-r--r--   0        0        0     4134 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py
+-rw-r--r--   0        0        0     6587 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py
+-rw-r--r--   0        0        0     6638 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py
+-rw-r--r--   0        0        0    15034 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py
+-rw-r--r--   0        0        0     9133 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py
+-rw-r--r--   0        0        0     2332 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py
+-rw-r--r--   0        0        0    64101 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py
+-rw-r--r--   0        0        0     1850 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py
+-rw-r--r--   0        0        0     4340 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py
+-rw-r--r--   0        0        0    15044 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py
+-rw-r--r--   0        0        0    11237 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py
+-rw-r--r--   0        0        0    24480 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/messari_model.py
+-rw-r--r--   0        0        0    22188 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/messari_view.py
+-rw-r--r--   0        0        0    25887 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py
+-rw-r--r--   0        0        0     8762 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py
+-rw-r--r--   0        0        0     3076 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py
+-rw-r--r--   0        0        0     2070 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py
+-rw-r--r--   0        0        0     2508 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py
+-rw-r--r--   0        0        0     6001 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py
+-rw-r--r--   0        0        0     3474 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/__init__.py
+-rw-r--r--   0        0        0     5562 2023-06-08 00:09:53.284146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nft_controller.py
+-rw-r--r--   0        0        0     1664 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py
+-rw-r--r--   0        0        0     4502 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py
+-rw-r--r--   0        0        0     2895 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/opensea_model.py
+-rw-r--r--   0        0        0     1289 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/opensea_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/__init__.py
+-rw-r--r--   0        0        0    21848 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/bitquery_model.py
+-rw-r--r--   0        0        0    11444 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/bitquery_view.py
+-rw-r--r--   0        0        0     3393 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/blockchain_model.py
+-rw-r--r--   0        0        0     4733 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/blockchain_view.py
+-rw-r--r--   0        0        0     1840 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py
+-rw-r--r--   0        0        0     1266 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py
+-rw-r--r--   0        0        0    15974 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py
+-rw-r--r--   0        0        0    10572 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py
+-rw-r--r--   0        0        0    50168 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/onchain_controller.py
+-rw-r--r--   0        0        0     6454 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/shroom_model.py
+-rw-r--r--   0        0        0     5953 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/shroom_view.py
+-rw-r--r--   0        0        0     4772 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py
+-rw-r--r--   0        0        0     2088 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/__init__.py
+-rw-r--r--   0        0        0     2274 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py
+-rw-r--r--   0        0        0     2427 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py
+-rw-r--r--   0        0        0     1464 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinbase_model.py
+-rw-r--r--   0        0        0     1342 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinbase_view.py
+-rw-r--r--   0        0        0    11841 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py
+-rw-r--r--   0        0        0     9646 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py
+-rw-r--r--   0        0        0     6776 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py
+-rw-r--r--   0        0        0     2278 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py
+-rw-r--r--   0        0        0     1100 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/glassnode_model.py
+-rw-r--r--   0        0        0     4677 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/glassnode_view.py
+-rw-r--r--   0        0        0     5936 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/loanscan_model.py
+-rw-r--r--   0        0        0     3279 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/loanscan_view.py
+-rw-r--r--   0        0        0    55381 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/overview_controller.py
+-rw-r--r--   0        0        0    13641 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py
+-rw-r--r--   0        0        0    21320 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py
+-rw-r--r--   0        0        0     5346 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/rekt_model.py
+-rw-r--r--   0        0        0     2253 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/rekt_view.py
+-rw-r--r--   0        0        0     2042 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/sdk_helpers.py
+-rw-r--r--   0        0        0     7167 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py
+-rw-r--r--   0        0        0     3126 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py
+-rw-r--r--   0        0        0     6708 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py
+-rw-r--r--   0        0        0     3480 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py
+-rw-r--r--   0        0        0     7635 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pycoingecko_helpers.py
+-rw-r--r--   0        0        0     5693 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pyth_model.py
+-rw-r--r--   0        0        0      973 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pyth_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26081 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    54572 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/__init__.py
+-rw-r--r--   0        0        0     6219 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_controller.py
+-rw-r--r--   0        0        0     1357 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_helpers.py
+-rw-r--r--   0        0        0     3447 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_model.py
+-rw-r--r--   0        0        0     2772 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_view.py
+-rw-r--r--   0        0        0    16935 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_prompt_toolkit.py
+-rw-r--r--   0        0        0    55138 2023-06-08 00:09:53.288146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/coin_highs.png
+-rw-r--r--   0        0        0  2879534 2023-06-08 00:09:53.304146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_crash.html
+-rw-r--r--   0        0        0   350260 2023-06-08 00:09:53.308146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_supply.png
+-rw-r--r--   0        0        0   607642 2023-06-08 00:09:53.312146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_terra.png
+-rw-r--r--   0        0        0    11988 2023-06-08 00:09:53.312146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb
+-rw-r--r--   0        0        0   667206 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/tvl.png
+-rw-r--r--   0        0        0   465754 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/ust_terra.png
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/__init__.py
+-rw-r--r--   0        0        0     9035 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/dashboards_controller.py
+-rw-r--r--   0        0        0    13578 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/Forecasting.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/__init__.py
+-rw-r--r--   0        0        0     3985 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/common_vars.py
+-rw-r--r--   0        0        0     4299 2023-06-08 00:09:53.316146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Chains.py
+-rw-r--r--   0        0        0     3366 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Correlation.py
+-rw-r--r--   0        0        0     8170 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Futures.py
+-rw-r--r--   0        0        0    17894 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Indicators.py
+-rw-r--r--   0        0        0     7008 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Short_Data.py
+-rw-r--r--   0        0        0    13262 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Stocks.py
+-rw-r--r--   0        0        0     4795 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/streamlit_helpers.py
+-rw-r--r--   0        0        0     1251 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/streamlit_run.py
+-rw-r--r--   0        0        0     5481 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/chains.ipynb
+-rw-r--r--   0        0        0     6789 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/correlation.ipynb
+-rw-r--r--   0        0        0    13930 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/forecast.ipynb
+-rw-r--r--   0        0        0    10953 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/futures.ipynb
+-rw-r--r--   0        0        0     9421 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/shortdata.ipynb
+-rw-r--r--   0        0        0    15315 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/stocks.ipynb
+-rw-r--r--   0        0        0     5091 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/decorators.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/__init__.py
+-rw-r--r--   0        0        0    83900 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_controller.py
+-rw-r--r--   0        0        0     2973 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_helpers.py
+-rw-r--r--   0        0        0    18675 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_model.py
+-rw-r--r--   0        0        0    20044 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_view.py
+-rw-r--r--   0        0        0    20449 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/regression_model.py
+-rw-r--r--   0        0        0     6739 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/regression_view.py
+-rw-r--r--   0        0        0       77 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/__init__.py
+-rw-r--r--   0        0        0    10230 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/alphavantage_model.py
+-rw-r--r--   0        0        0    12117 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/alphavantage_view.py
+-rw-r--r--   0        0        0     1890 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/commodity_model.py
+-rw-r--r--   0        0        0     1569 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/commodity_view.py
+-rw-r--r--   0        0        0      909 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv
+-rw-r--r--   0        0        0    21218 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/cpi.csv
+-rw-r--r--   0        0        0    10355 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/harmonized_cpi.csv
+-rw-r--r--   0        0        0    28404 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/econdb_model.py
+-rw-r--r--   0        0        0     8027 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/econdb_view.py
+-rw-r--r--   0        0        0    90104 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/economy_controller.py
+-rw-r--r--   0        0        0     3436 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/economy_helpers.py
+-rw-r--r--   0        0        0     8043 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/finviz_model.py
+-rw-r--r--   0        0        0     3837 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/finviz_view.py
+-rw-r--r--   0        0        0     9940 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/fred_model.py
+-rw-r--r--   0        0        0     9124 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/fred_view.py
+-rw-r--r--   0        0        0     6972 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/nasdaq_model.py
+-rw-r--r--   0        0        0     3293 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/nasdaq_view.py
+-rw-r--r--   0        0        0    38618 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/oecd_model.py
+-rw-r--r--   0        0        0    28284 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/oecd_view.py
+-rw-r--r--   0        0        0     3768 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/plot_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    28433 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1218 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/sdk_helpers.py
+-rw-r--r--   0        0        0    12870 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/wsj_model.py
+-rw-r--r--   0        0        0     4673 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/wsj_view.py
+-rw-r--r--   0        0        0    30415 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/yfinance_model.py
+-rw-r--r--   0        0        0     5062 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/yfinance_view.py
+-rw-r--r--   0        0        0      106 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/__init__.py
+-rw-r--r--   0        0        0     4023 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/disc_controller.py
+-rw-r--r--   0        0        0     2804 2023-06-08 00:09:53.320146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/wsj_model.py
+-rw-r--r--   0        0        0     1320 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/wsj_view.py
+-rw-r--r--   0        0        0    21045 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/etf_controller.py
+-rw-r--r--   0        0        0      450 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/etf_helper.py
+-rw-r--r--   0        0        0   188615 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/etfs.csv
+-rw-r--r--   0        0        0     2608 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/financedatabase_model.py
+-rw-r--r--   0        0        0     3864 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/financedatabase_view.py
+-rw-r--r--   0        0        0     1417 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/fmp_model.py
+-rw-r--r--   0        0        0     3152 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/fmp_view.py
+-rw-r--r--   0        0        0     4172 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/stockanalysis_model.py
+-rw-r--r--   0        0        0     3941 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/stockanalysis_view.py
+-rw-r--r--   0        0        0    51458 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     6229 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/featflags_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/__init__.py
+-rw-r--r--   0        0        0    58622 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/corporate_spot_rates.csv
+-rw-r--r--   0        0        0     9217 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     7103 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ecb_view.py
+-rw-r--r--   0        0        0     5811 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/econdb_model.py
+-rw-r--r--   0        0        0     7831 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/econdb_view.py
+-rw-r--r--   0        0        0    56238 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0    38003 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fred_model.py
+-rw-r--r--   0        0        0    55506 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fred_view.py
+-rw-r--r--   0        0        0   227110 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ice_bofa_indices.csv
+-rw-r--r--   0        0        0    10963 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/oecd_model.py
+-rw-r--r--   0        0        0     4004 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/oecd_view.py
+-rw-r--r--   0        0        0     2174 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/yfinance_model.py
+-rw-r--r--   0        0        0     1702 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-08 00:09:53.324146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/anom_model.py
+-rw-r--r--   0        0        0     2962 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/anom_view.py
+-rw-r--r--   0        0        0     4629 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoarima_model.py
+-rw-r--r--   0        0        0     3933 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoarima_view.py
+-rw-r--r--   0        0        0     4658 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoces_model.py
+-rw-r--r--   0        0        0     3970 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoces_view.py
+-rw-r--r--   0        0        0     4694 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoets_model.py
+-rw-r--r--   0        0        0     3972 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoets_view.py
+-rw-r--r--   0        0        0     7567 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoselect_model.py
+-rw-r--r--   0        0        0     3938 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoselect_view.py
+-rw-r--r--   0        0        0     5874 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/brnn_model.py
+-rw-r--r--   0        0        0     6577 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/brnn_view.py
+-rw-r--r--   0        0        0     5562 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/expo_model.py
+-rw-r--r--   0        0        0     5038 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/expo_view.py
+-rw-r--r--   0        0        0     2053 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast.ipynb
+-rw-r--r--   0        0        0   121975 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_controller.py
+-rw-r--r--   0        0        0    15471 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_model.py
+-rw-r--r--   0        0        0     9034 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_view.py
+-rw-r--r--   0        0        0    47145 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/helpers.py
+-rw-r--r--   0        0        0     3405 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/linregr_model.py
+-rw-r--r--   0        0        0     4760 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/linregr_view.py
+-rw-r--r--   0        0        0     5013 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/mstl_model.py
+-rw-r--r--   0        0        0     3861 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/mstl_view.py
+-rw-r--r--   0        0        0     5896 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nbeats_model.py
+-rw-r--r--   0        0        0     6396 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nbeats_view.py
+-rw-r--r--   0        0        0     7561 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nhits_model.py
+-rw-r--r--   0        0        0     7952 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nhits_view.py
+-rw-r--r--   0        0        0     3007 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/regr_model.py
+-rw-r--r--   0        0        0     4521 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/regr_view.py
+-rw-r--r--   0        0        0     5030 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rnn_model.py
+-rw-r--r--   0        0        0     5533 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rnn_view.py
+-rw-r--r--   0        0        0     4340 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rwd_model.py
+-rw-r--r--   0        0        0     3643 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rwd_view.py
+-rw-r--r--   0        0        0     4709 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/seasonalnaive_model.py
+-rw-r--r--   0        0        0     3879 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/seasonalnaive_view.py
+-rw-r--r--   0        0        0     5790 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tcn_model.py
+-rw-r--r--   0        0        0     6289 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tcn_view.py
+-rw-r--r--   0        0        0     7249 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tft_model.py
+-rw-r--r--   0        0        0     6520 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tft_view.py
+-rw-r--r--   0        0        0     4928 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/theta_model.py
+-rw-r--r--   0        0        0     4379 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/theta_view.py
+-rw-r--r--   0        0        0     6321 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/trans_model.py
+-rw-r--r--   0        0        0     6765 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/trans_view.py
+-rw-r--r--   0        0        0    12580 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/whisper_model.py
+-rw-r--r--   0        0        0     2935 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/whisper_utils.py
+-rw-r--r--   0        0        0      122 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/__init__.py
+-rw-r--r--   0        0        0     5050 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/av_model.py
+-rw-r--r--   0        0        0     1458 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/av_view.py
+-rw-r--r--   0        0        0     3281 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/av_forex_currencies.csv
+-rw-r--r--   0        0        0     7847 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/polygon_tickers.csv
+-rw-r--r--   0        0        0   419838 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/yahoofinance_forex.json
+-rw-r--r--   0        0        0    16492 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/forex_controller.py
+-rw-r--r--   0        0        0     8201 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/forex_helper.py
+-rw-r--r--   0        0        0      931 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/fxempire_model.py
+-rw-r--r--   0        0        0     1471 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/fxempire_view.py
+-rw-r--r--   0        0        0    17162 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_controller.py
+-rw-r--r--   0        0        0    22592 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_model.py
+-rw-r--r--   0        0        0    12856 2023-06-08 00:09:53.328146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_view.py
+-rw-r--r--   0        0        0     2349 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/polygon_model.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0    26168 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0     1446 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/sdk_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/technical_analysis/__init__.py
+-rw-r--r--   0        0        0    35136 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/__init__.py
+-rw-r--r--   0        0        0     2225 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/databento_view.py
+-rw-r--r--   0        0        0     9653 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/futures_controller.py
+-rw-r--r--   0        0        0      358 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/futures_helper.py
+-rw-r--r--   0        0        0      964 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/sdk_helper.py
+-rw-r--r--   0        0        0     5669 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/yfinance_model.py
+-rw-r--r--   0        0        0     8070 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/yfinance_view.py
+-rw-r--r--   0        0        0    13050 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/helper_classes.py
+-rw-r--r--   0        0        0    63148 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/helper_funcs.py
+-rw-r--r--   0        0        0     3212 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/helpers_denomination.py
+-rw-r--r--   0        0        0     9743 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/intro.json
+-rw-r--r--   0        0        0    45225 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_controller.py
+-rw-r--r--   0        0        0    80064 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_model.py
+-rw-r--r--   0        0        0     1148 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_view.py
+-rw-r--r--   0        0        0    11456 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/loggers.py
+-rw-r--r--   0        0        0     1701 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/menu.py
+-rw-r--r--   0        0        0    23784 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.csv
+-rw-r--r--   0        0        0    29952 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.json
+-rw-r--r--   0        0        0     6403 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.csv
+-rw-r--r--   0        0        0     8797 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.json
+-rw-r--r--   0        0        0    11455 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/generate_documentation_commands.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/alternative/covid/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/common/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/common/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/common/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/common/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/custom/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/econometrics/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/economy/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/etf/movers/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/etf/screeners/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/mutual_funds/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/portfolio/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/portfolio/views/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/backtesting/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/behavioural_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/comparison_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/dark_pool_shorts/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/discovery/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/due_diligence/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/fundamental_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/government/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/insider/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/options/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/prediction_techniques/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/quantitative_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/raw_data/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/sector_industry_analysis/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/exports/stocks/technical_analysis/.gitkeep
+-rw-r--r--   0        0        0     8528 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/futures/futures.csv
+-rw-r--r--   0        0        0    60375 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/i18n/en.yml
+-rw-r--r--   0        0        0     5831 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/i18n/help_translation.ipynb
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/.gitkeep
+-rw-r--r--   0        0        0     3868 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD
+-rw-r--r--   0        0        0      101 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/account/test_account.openbb
+-rw-r--r--   0        0        0       66 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_alt.openbb
+-rw-r--r--   0        0        0       87 2023-06-08 00:09:53.332146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_covid.openbb
+-rw-r--r--   0        0        0      164 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_oss.openbb
+-rw-r--r--   0        0        0      209 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/alternative/test_realestate.openbb
+-rw-r--r--   0        0        0      936 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb
+-rw-r--r--   0        0        0     1039 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_dd.openbb
+-rw-r--r--   0        0        0     1319 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_defi.openbb
+-rw-r--r--   0        0        0      582 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_discovery.openbb
+-rw-r--r--   0        0        0      195 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_nft.openbb
+-rw-r--r--   0        0        0     1287 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_onchain.openbb
+-rw-r--r--   0        0        0     1606 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_overview.openbb
+-rw-r--r--   0        0        0      604 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_qa.openbb
+-rw-r--r--   0        0        0      850 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_ta.openbb
+-rw-r--r--   0        0        0      165 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_tools.openbb
+-rw-r--r--   0        0        0      132 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/dashboards/test_dashboards.openbb
+-rw-r--r--   0        0        0     1440 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics.openbb
+-rw-r--r--   0        0        0     2436 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb
+-rw-r--r--   0        0        0      274 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_qa.openbb
+-rw-r--r--   0        0        0       41 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ca.openbb
+-rw-r--r--   0        0        0      265 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_disc.openbb
+-rw-r--r--   0        0        0      227 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_etf.openbb
+-rw-r--r--   0        0        0      890 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ta.openbb
+-rw-r--r--   0        0        0     2301 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb
+-rw-r--r--   0        0        0      521 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb
+-rw-r--r--   0        0        0      449 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_forex.openbb
+-rw-r--r--   0        0        0      791 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_oanda.openbb
+-rw-r--r--   0        0        0      654 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_qa.openbb
+-rw-r--r--   0        0        0      636 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_ta.openbb
+-rw-r--r--   0        0        0      184 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/futures/test_futures.openbb
+-rw-r--r--   0        0        0       16 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/keys/test_keys.openbb
+-rw-r--r--   0        0        0      277 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/mutual_funds/test_mutual_fund.openbb
+-rw-r--r--   0        0        0      109 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_params.openbb
+-rw-r--r--   0        0        0     1967 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po.openbb
+-rw-r--r--   0        0        0     1850 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb
+-rw-r--r--   0        0        0      509 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/reports/test_reports.openbb
+-rw-r--r--   0        0        0      272 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ba.openbb
+-rw-r--r--   0        0        0     1524 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_bt.openbb
+-rw-r--r--   0        0        0      635 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ca.openbb
+-rw-r--r--   0        0        0      282 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_disc.openbb
+-rw-r--r--   0        0        0      177 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_dps.openbb
+-rw-r--r--   0        0        0     1741 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_fa.openbb
+-rw-r--r--   0        0        0       21 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_forecast.openbb
+-rw-r--r--   0        0        0      481 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_gov.openbb
+-rw-r--r--   0        0        0      154 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_hedge.openbb
+-rw-r--r--   0        0        0      236 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_insider.openbb
+-rw-r--r--   0        0        0      361 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_options.openbb
+-rw-r--r--   0        0        0      671 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_qa.openbb
+-rw-r--r--   0        0        0       47 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_res.openbb
+-rw-r--r--   0        0        0      163 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_screener.openbb
+-rw-r--r--   0        0        0      735 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb
+-rw-r--r--   0        0        0      768 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ta.openbb
+-rw-r--r--   0        0        0      102 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_tradinghours.openbb
+-rw-r--r--   0        0        0       46 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/terminal/test_news.openbb
+-rw-r--r--   0        0        0     1065 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/models/hub_credentials.json
+-rw-r--r--   0        0        0      380 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/models/local_credentials.json
+-rw-r--r--   0        0        0    17970 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx
+-rw-r--r--   0        0        0    29757 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx
+-rw-r--r--   0        0        0    33733 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/parameters_template.xlsx
+-rw-r--r--   0        0        0      310 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/routines/routine_example.openbb
+-rw-r--r--   0        0        0    21793 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/sources/openbb_default.json
+-rw-r--r--   0        0        0     2332 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini
+-rw-r--r--   0        0        0     2354 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini
+-rw-r--r--   0        0        0     2341 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini
+-rw-r--r--   0        0        0     2316 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini
+-rw-r--r--   0        0        0     2316 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Banks.ini
+-rw-r--r--   0        0        0     2346 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini
+-rw-r--r--   0        0        0     2336 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini
+-rw-r--r--   0        0        0     2346 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini
+-rw-r--r--   0        0        0     2307 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini
+-rw-r--r--   0        0        0     2309 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Construction.ini
+-rw-r--r--   0        0        0     2329 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini
+-rw-r--r--   0        0        0     2353 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini
+-rw-r--r--   0        0        0     2360 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini
+-rw-r--r--   0        0        0     2320 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini
+-rw-r--r--   0        0        0     2344 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini
+-rw-r--r--   0        0        0     2315 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini
+-rw-r--r--   0        0        0     2346 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini
+-rw-r--r--   0        0        0     2376 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini
+-rw-r--r--   0        0        0     2326 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Health.ini
+-rw-r--r--   0        0        0     2307 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini
+-rw-r--r--   0        0        0     2320 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini
+-rw-r--r--   0        0        0     2324 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini
+-rw-r--r--   0        0        0     2334 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini
+-rw-r--r--   0        0        0     2324 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Legal.ini
+-rw-r--r--   0        0        0     2313 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini
+-rw-r--r--   0        0        0     2341 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini
+-rw-r--r--   0        0        0     2296 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Mining.ini
+-rw-r--r--   0        0        0     2367 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini
+-rw-r--r--   0        0        0     2342 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini
+-rw-r--r--   0        0        0     2361 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini
+-rw-r--r--   0        0        0     2351 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini
+-rw-r--r--   0        0        0     2336 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini
+-rw-r--r--   0        0        0     2322 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini
+-rw-r--r--   0        0        0     2310 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini
+-rw-r--r--   0        0        0     2326 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini
+-rw-r--r--   0        0        0     2341 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini
+-rw-r--r--   0        0        0     2299 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini
+-rw-r--r--   0        0        0     2316 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini
+-rw-r--r--   0        0        0     2342 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini
+-rw-r--r--   0        0        0     2381 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini
+-rw-r--r--   0        0        0     2314 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini
+-rw-r--r--   0        0        0    34473 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/template.ini
+-rw-r--r--   0        0        0    34519 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/whales.ini
+-rwxr-xr-x   0        0        0      282 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/5pct_above_low.ini
+-rw-r--r--   0        0        0    21940 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt
+-rwxr-xr-x   0        0        0      315 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/analyst_strong_buy.ini
+-rwxr-xr-x   0        0        0      464 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/break_out_stocks.ini
+-rw-r--r--   0        0        0      413 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/buffett_like.ini
+-rwxr-xr-x   0        0        0      184 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/bull_runs_over_10pct.ini
+-rwxr-xr-x   0        0        0      364 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/channel_up_and_low_debt_and_sma_50and200.ini
+-rw-r--r--   0        0        0      326 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/cheap_bottom_dividend.ini
+-rw-r--r--   0        0        0      193 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/cheap_dividend.ini
+-rw-r--r--   0        0        0      241 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/cheap_oversold.ini
+-rwxr-xr-x   0        0        0      335 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/continued_momentum_scan.ini
+-rw-r--r--   0        0        0      286 2023-06-08 00:09:53.336146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/death_cross.ini
+-rwxr-xr-x   0        0        0      167 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/djia_components.ini
+-rw-r--r--   0        0        0      221 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/golden_cross.ini
+-rwxr-xr-x   0        0        0      255 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/golden_cross_penny.ini
+-rwxr-xr-x   0        0        0      518 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini
+-rw-r--r--   0        0        0      302 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/heavy_inst_ins.ini
+-rwxr-xr-x   0        0        0      279 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/high_vol_and_low_debt.ini
+-rw-r--r--   0        0        0      316 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/modified_dreman.ini
+-rw-r--r--   0        0        0      349 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/modified_neff.ini
+-rwxr-xr-x   0        0        0      295 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/news_scanner.ini
+-rwxr-xr-x   0        0        0      274 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/oversold.ini
+-rwxr-xr-x   0        0        0      328 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/oversold_under_3dol.ini
+-rwxr-xr-x   0        0        0      301 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/oversold_under_5dol.ini
+-rwxr-xr-x   0        0        0      212 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/potential_reversals.ini
+-rwxr-xr-x   0        0        0      295 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/recent_growth_and_support.ini
+-rw-r--r--   0        0        0      337 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/rosenwald.ini
+-rw-r--r--   0        0        0      280 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/rosenwald_gtfo.ini
+-rw-r--r--   0        0        0      246 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sdk_guide_preset.ini
+-rw-r--r--   0        0        0      360 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sexy_year.ini
+-rwxr-xr-x   0        0        0      222 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/short_squeeze_scan.ini
+-rwxr-xr-x   0        0        0      260 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/simplistic_momentum_scanner_under_7dol.ini
+-rwxr-xr-x   0        0        0      197 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_basic_materials_sector.ini
+-rwxr-xr-x   0        0        0      211 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_communication_services_sector.ini
+-rwxr-xr-x   0        0        0      201 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_cyclical_sector.ini
+-rwxr-xr-x   0        0        0      203 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_consumer_defensive_sector.ini
+-rwxr-xr-x   0        0        0      179 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_energy_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_financial_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_healthcare_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_industrials_sector.ini
+-rwxr-xr-x   0        0        0      189 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_real_estate_sector.ini
+-rwxr-xr-x   0        0        0      187 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_technology_sector.ini
+-rwxr-xr-x   0        0        0      185 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/sp500_utilities_sector.ini
+-rwxr-xr-x   0        0        0      276 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/stocks_strong_support_levels.ini
+-rwxr-xr-x   0        0        0      272 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/top_performers_all.ini
+-rwxr-xr-x   0        0        0      299 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/top_performers_healthcare.ini
+-rwxr-xr-x   0        0        0      293 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/top_performers_tech.ini
+-rwxr-xr-x   0        0        0      286 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/under_15dol_stocks.ini
+-rw-r--r--   0        0        0      209 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/undervalue.ini
+-rwxr-xr-x   0        0        0      272 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/unusual_volume.ini
+-rwxr-xr-x   0        0        0      675 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini
+-rwxr-xr-x   0        0        0      315 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/weak_support_and_top_performers.ini
+-rw-r--r--   0        0        0   358460 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/Consolas.ttf
+-rw-r--r--   0        0        0      972 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.mplrc.json
+-rw-r--r--   0        0        0     2086 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.mplstyle
+-rw-r--r--   0        0        0     2750 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0      203 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.richstyle.json
+-rw-r--r--   0        0        0      970 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json
+-rw-r--r--   0        0        0      182 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.mplrc.json
+-rw-r--r--   0        0        0     2035 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.mplstyle
+-rw-r--r--   0        0        0    24193 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0      202 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.richstyle.json
+-rw-r--r--   0        0        0     2607 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0      186 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/user/openbb.richstyle.json
+-rw-r--r--   0        0        0      144 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.340146 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/__init__.py
+-rw-r--r--   0        0        0    81373 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_fund_ID.csv
+-rw-r--r--   0        0        0      834 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_model.py
+-rw-r--r--   0        0        0     3941 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_view.py
+-rw-r--r--   0        0        0     6535 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mstarpy_model.py
+-rw-r--r--   0        0        0     7883 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mstarpy_view.py
+-rw-r--r--   0        0        0    15141 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mutual_fund_controller.py
+-rw-r--r--   0        0        0     6040 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mutual_funds_utils.py
+-rw-r--r--   0        0        0    50383 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/parent_classes.py
+-rw-r--r--   0        0        0       61 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/__init__.py
+-rw-r--r--   0        0        0    15080 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/allocation_model.py
+-rw-r--r--   0        0        0    12944 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/attribution_model.py
+-rw-r--r--   0        0        0      417 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/__init__.py
+-rw-r--r--   0        0        0     3214 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/bro_controller.py
+-rw-r--r--   0        0        0     1121 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/brokers_helpers.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/__init__.py
+-rw-r--r--   0        0        0     8211 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py
+-rw-r--r--   0        0        0     9561 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py
+-rw-r--r--   0        0        0     4495 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py
+-rw-r--r--   0        0        0     4666 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/__init__.py
+-rw-r--r--   0        0        0    12789 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py
+-rw-r--r--   0        0        0    15571 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_model.py
+-rw-r--r--   0        0        0    15670 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_view.py
+-rw-r--r--   0        0        0     3894 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py
+-rw-r--r--   0        0        0     3002 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py
+-rw-r--r--   0        0        0     2482 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py
+-rw-r--r--   0        0        0    30861 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/metrics_model.py
+-rw-r--r--   0        0        0    54979 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_controller.py
+-rw-r--r--   0        0        0    39188 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_engine.py
+-rw-r--r--   0        0        0     9643 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_helper.py
+-rw-r--r--   0        0        0    60205 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_model.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/__init__.py
+-rw-r--r--   0        0        0     5255 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/excel_model.py
+-rw-r--r--   0        0        0     2106 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py
+-rw-r--r--   0        0        0   120571 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py
+-rw-r--r--   0        0        0   155050 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py
+-rw-r--r--   0        0        0     2773 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py
+-rw-r--r--   0        0        0    13116 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py
+-rw-r--r--   0        0        0     5974 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py
+-rw-r--r--   0        0        0     5346 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py
+-rw-r--r--   0        0        0     4427 2023-06-08 00:09:53.344147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py
+-rw-r--r--   0        0        0   138034 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_controller.py
+-rw-r--r--   0        0        0     8587 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_engine.py
+-rw-r--r--   0        0        0   103568 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_model.py
+-rw-r--r--   0        0        0    24186 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_view.py
+-rw-r--r--   0        0        0    11390 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/statics.py
+-rw-r--r--   0        0        0    12009 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py
+-rw-r--r--   0        0        0    54951 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_view.py
+-rw-r--r--   0        0        0     8433 2023-06-08 00:09:53.348147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/statics.py
+-rw-r--r--   0        0        0  1028287 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html
+-rw-r--r--   0        0        0     2839 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/__init__.py
+-rw-r--r--   0        0        0      443 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/data/crypto_tickers.csv
+-rw-r--r--   0        0        0      437 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/data/etf_tickers.csv
+-rw-r--r--   0        0        0      222 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/data/stocks_tickers.csv
+-rw-r--r--   0        0        0     9706 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/reports_controller.py
+-rw-r--r--   0        0        0    12310 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/reports_model.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.352147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/stored/.gitkeep
+-rw-r--r--   0        0        0  1076317 2023-06-08 00:09:53.356147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html
+-rw-r--r--   0        0        0     5214 2023-06-08 00:09:53.356147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/OpenBB_reports_logo.png
+-rw-r--r--   0        0        0    32656 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/crypto.ipynb
+-rw-r--r--   0        0        0    25803 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/economy.ipynb
+-rw-r--r--   0        0        0    40287 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/equity.ipynb
+-rw-r--r--   0        0        0    13582 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/etf.ipynb
+-rw-r--r--   0        0        0     2782 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/floppy-disc.png
+-rw-r--r--   0        0        0     8567 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/forecast.ipynb
+-rw-r--r--   0        0        0    17778 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/forex.ipynb
+-rw-r--r--   0        0        0    14922 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/portfolio.ipynb
+-rw-r--r--   0        0        0    11247 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widget_helpers.py
+-rw-r--r--   0        0        0      205 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/card.j2
+-rw-r--r--   0        0        0     3556 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/report.css
+-rw-r--r--   0        0        0      474 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/report.j2
+-rw-r--r--   0        0        0      119 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/row.j2
+-rw-r--r--   0        0        0      896 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/style.css
+-rw-r--r--   0        0        0     9967 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/rich_config.py
+-rw-r--r--   0        0        0    20276 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/routine_functions.py
+-rw-r--r--   0        0        0    31224 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/sdk.py
+-rw-r--r--   0        0        0    20375 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/settings_controller.py
+-rw-r--r--   0        0        0     7105 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/sources_controller.py
+-rw-r--r--   0        0        0      357 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/__init__.py
+-rw-r--r--   0        0        0    10448 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_controller.py
+-rw-r--r--   0        0        0     8126 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_model.py
+-rw-r--r--   0        0        0     9046 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/__init__.py
+-rw-r--r--   0        0        0    29872 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/ba_controller.py
+-rw-r--r--   0        0        0     3541 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3761 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     1931 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/cboe_model.py
+-rw-r--r--   0        0        0      969 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/cboe_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/__init__.py
+-rw-r--r--   0        0        0    37621 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/ca_controller.py
+-rw-r--r--   0        0        0     4871 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finbrain_model.py
+-rw-r--r--   0        0        0     5859 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1328 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     2738 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py
+-rw-r--r--   0        0        0     1539 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py
+-rw-r--r--   0        0        0    12451 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     5957 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     1690 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/polygon_model.py
+-rw-r--r--   0        0        0     1379 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0     8073 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    10164 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/__init__.py
+-rw-r--r--   0        0        0    20377 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py
+-rw-r--r--   0        0        0     9982 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/finra_model.py
+-rw-r--r--   0        0        0     7203 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/finra_view.py
+-rw-r--r--   0        0        0     1093 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py
+-rw-r--r--   0        0        0     1200 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py
+-rw-r--r--   0        0        0     1387 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py
+-rw-r--r--   0        0        0     4816 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py
+-rw-r--r--   0        0        0     6836 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/sec_model.py
+-rw-r--r--   0        0        0     3477 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/sec_view.py
+-rw-r--r--   0        0        0     1882 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py
+-rw-r--r--   0        0        0     1385 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py
+-rw-r--r--   0        0        0     5053 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py
+-rw-r--r--   0        0        0     9997 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py
+-rw-r--r--   0        0        0     1166 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py
+-rw-r--r--   0        0        0     3769 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py
+-rw-r--r--   0        0        0      668 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py
+-rw-r--r--   0        0        0     1271 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py
+-rw-r--r--   0        0        0     4421 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/databento_model.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/__init__.py
+-rw-r--r--   0        0        0     4169 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/ark_model.py
+-rw-r--r--   0        0        0     2589 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/ark_view.py
+-rw-r--r--   0        0        0    29463 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/disc_controller.py
+-rw-r--r--   0        0        0      483 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/disc_helpers.py
+-rw-r--r--   0        0        0     2696 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fidelity_model.py
+-rw-r--r--   0        0        0     2610 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fidelity_view.py
+-rw-r--r--   0        0        0     4164 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finnhub_model.py
+-rw-r--r--   0        0        0     2510 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finnhub_view.py
+-rw-r--r--   0        0        0     1731 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finviz_model.py
+-rw-r--r--   0        0        0     3084 2023-06-08 00:09:53.360147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finviz_view.py
+-rw-r--r--   0        0        0     2562 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fmp_view.py
+-rw-r--r--   0        0        0     3051 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/nasdaq_model.py
+-rw-r--r--   0        0        0     3406 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/nasdaq_view.py
+-rw-r--r--   0        0        0     5934 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/seeking_alpha_model.py
+-rw-r--r--   0        0        0     3485 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/seeking_alpha_view.py
+-rw-r--r--   0        0        0     1120 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/shortinterest_model.py
+-rw-r--r--   0        0        0     2566 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/shortinterest_view.py
+-rw-r--r--   0        0        0     4113 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/yahoofinance_model.py
+-rw-r--r--   0        0        0     5871 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/yahoofinance_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/__init__.py
+-rw-r--r--   0        0        0    24126 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/av_model.py
+-rw-r--r--   0        0        0    14922 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/av_view.py
+-rw-r--r--   0        0        0     8170 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py
+-rw-r--r--   0        0        0     7775 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py
+-rw-r--r--   0        0        0     1833 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py
+-rw-r--r--   0        0        0     2347 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py
+-rw-r--r--   0        0        0    14744 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_model.py
+-rw-r--r--   0        0        0     4279 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_static.py
+-rw-r--r--   0        0        0    44494 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_view.py
+-rw-r--r--   0        0        0     1925 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py
+-rw-r--r--   0        0        0     1205 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py
+-rw-r--r--   0        0        0     2396 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py
+-rw-r--r--   0        0        0     4904 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py
+-rw-r--r--   0        0        0    81997 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fa_controller.py
+-rw-r--r--   0        0        0      266 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fa_helper.py
+-rw-r--r--   0        0        0     1389 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py
+-rw-r--r--   0        0        0     3518 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py
+-rw-r--r--   0        0        0     3478 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finviz_model.py
+-rw-r--r--   0        0        0     2484 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finviz_view.py
+-rw-r--r--   0        0        0    22344 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fmp_model.py
+-rw-r--r--   0        0        0    23771 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fmp_view.py
+-rw-r--r--   0        0        0     6417 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt
+-rw-r--r--   0        0        0    11893 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py
+-rw-r--r--   0        0        0     1350 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py
+-rw-r--r--   0        0        0     2654 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/nasdaq_model.py
+-rw-r--r--   0        0        0     1862 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/nasdaq_view.py
+-rw-r--r--   0        0        0     5391 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/polygon_model.py
+-rw-r--r--   0        0        0     4360 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/polygon_view.py
+-rw-r--r--   0        0        0     8546 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py
+-rw-r--r--   0        0        0    11162 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py
+-rw-r--r--   0        0        0     2059 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py
+-rw-r--r--   0        0        0    11817 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py
+-rw-r--r--   0        0        0    14162 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/__init__.py
+-rw-r--r--   0        0        0    18461 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/gov_controller.py
+-rw-r--r--   0        0        0    15719 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/quiverquant_model.py
+-rw-r--r--   0        0        0    21428 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/quiverquant_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/__init__.py
+-rw-r--r--   0        0        0     2062 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/businessinsider_model.py
+-rw-r--r--   0        0        0     5102 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/businessinsider_view.py
+-rw-r--r--   0        0        0     1125 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/finviz_model.py
+-rw-r--r--   0        0        0     1171 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/finviz_view.py
+-rw-r--r--   0        0        0    32744 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/insider_controller.py
+-rw-r--r--   0        0        0    87495 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/openinsider_model.py
+-rw-r--r--   0        0        0     7695 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/openinsider_view.py
+-rw-r--r--   0        0        0     4909 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/sdk_helper.py
+-rw-r--r--   0        0        0    76085 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/mappings/Mic_Codes.csv
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-08 00:09:53.364147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/alphaquery_model.py
+-rw-r--r--   0        0        0     1713 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/alphaquery_view.py
+-rw-r--r--   0        0        0     1161 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/barchart_model.py
+-rw-r--r--   0        0        0     1137 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/barchart_view.py
+-rw-r--r--   0        0        0     1526 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/calculator_model.py
+-rw-r--r--   0        0        0     2416 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/calculator_view.py
+-rw-r--r--   0        0        0     2777 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/chartexchange_model.py
+-rw-r--r--   0        0        0     3271 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/chartexchange_view.py
+-rw-r--r--   0        0        0     2433 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/fdscanner_model.py
+-rw-r--r--   0        0        0     1672 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/fdscanner_view.py
+-rw-r--r--   0        0        0    21092 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_controller.py
+-rw-r--r--   0        0        0     9884 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_model.py
+-rw-r--r--   0        0        0     3968 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_view.py
+-rw-r--r--   0        0        0    10111 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/intrinio_model.py
+-rw-r--r--   0        0        0     6390 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/intrinio_view.py
+-rw-r--r--   0        0        0     7070 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/nasdaq_model.py
+-rw-r--r--   0        0        0    17467 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/op_helpers.py
+-rw-r--r--   0        0        0    51114 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_controller.py
+-rw-r--r--   0        0        0     9034 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_sdk_helper.py
+-rw-r--r--   0        0        0    14494 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_view.py
+-rw-r--r--   0        0        0     8410 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/tradier_model.py
+-rw-r--r--   0        0        0     2903 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/tradier_view.py
+-rw-r--r--   0        0        0     7647 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/yfinance_model.py
+-rw-r--r--   0        0        0    11535 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/yfinance_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/__init__.py
+-rw-r--r--   0        0        0     2260 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/beta_model.py
+-rw-r--r--   0        0        0     2798 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/beta_view.py
+-rw-r--r--   0        0        0     3187 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/factors_model.py
+-rw-r--r--   0        0        0      687 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/factors_view.py
+-rw-r--r--   0        0        0    38741 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/qa_controller.py
+-rw-r--r--   0        0        0      447 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/qa_model.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/research/__init__.py
+-rw-r--r--   0        0        0     6218 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/research/res_controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/__init__.py
+-rw-r--r--   0        0        0    46671 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/finviz_model.py
+-rw-r--r--   0        0        0     7192 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/finviz_view.py
+-rw-r--r--   0        0        0    21493 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_controller.py
+-rw-r--r--   0        0        0      944 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_helper.py
+-rw-r--r--   0        0        0     2562 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_view.py
+-rw-r--r--   0        0        0    27722 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stock_statics.py
+-rw-r--r--   0        0        0    28108 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_controller.py
+-rw-r--r--   0        0        0    35085 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_helper.py
+-rw-r--r--   0        0        0    11340 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_model.py
+-rw-r--r--   0        0        0     1559 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/__init__.py
+-rw-r--r--   0        0        0     1004 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/finbrain_model.py
+-rw-r--r--   0        0        0      644 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/finbrain_view.py
+-rw-r--r--   0        0        0     1532 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/rsp_model.py
+-rw-r--r--   0        0        0     2386 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/rsp_view.py
+-rw-r--r--   0        0        0    65324 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/ta_controller.py
+-rw-r--r--   0        0        0     3260 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/tradingview_model.py
+-rw-r--r--   0        0        0     1985 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/tradingview_view.py
+-rw-r--r--   0        0        0      334 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/README.md
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/__init__.py
+-rw-r--r--   0        0        0     5328 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/bursa_model.py
+-rw-r--r--   0        0        0     2202 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/bursa_view.py
+-rw-r--r--   0        0        0        0 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/data/__init__.py
+-rw-r--r--   0        0        0    28098 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json
+-rw-r--r--   0        0        0     1466 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py
+-rw-r--r--   0        0        0     1378 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py
+-rw-r--r--   0        0        0    10137 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/tradinghours_controller.py
+-rw-r--r--   0        0        0      614 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/tradinghours_helper.py
+-rw-r--r--   0        0        0    42676 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/terminal_controller.py
+-rw-r--r--   0        0        0    14590 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/terminal_helper.py
+-rw-r--r--   0        0        0     3848 2023-06-08 00:09:53.368147 openbb_nightly-3.0.1.dev20230608/openbb_terminal/thought_of_the_day.py
+-rw-r--r--   0        0        0     5737 2023-06-08 00:09:55.104170 openbb_nightly-3.0.1.dev20230608/pyproject.toml
+-rw-r--r--   0        0        0     1145 2023-06-08 00:09:53.372147 openbb_nightly-3.0.1.dev20230608/terminal.py
+-rw-r--r--   0        0        0     2285 2023-06-08 00:09:55.108171 openbb_nightly-3.0.1.dev20230608/website/pypi.md
+-rw-r--r--   0        0        0     7785 1970-01-01 00:00:00.000000 openbb_nightly-3.0.1.dev20230608/PKG-INFO
```

### Comparing `openbb_nightly-3.0.1.dev20230607/LICENSE` & `openbb_nightly-3.0.1.dev20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/account_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/account_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/account/account_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/account/account_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/alt_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/alt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/countries.txt` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/countries.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/covid/covid_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/covid/covid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/hackernews_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/hackernews_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/hackernews_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/hackernews_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/github_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/github_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/github_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/github_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/oss_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/oss_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/runa_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/runa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/oss/runa_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/oss/runa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/landRegistry_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/landRegistry_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/landRegistry_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/landRegistry_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/alternative/realestate/realestate_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/alternative/realestate/realestate_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/base_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/base_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finbrain_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finbrain_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/google_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/google_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/google_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/google_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/reddit_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/reddit_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/stocktwits_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/stocktwits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/stocktwits_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/stocktwits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/twitter_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/twitter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/behavioural_analysis/twitter_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/behavioural_analysis/twitter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/biztoc_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/biztoc_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/biztoc_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/biztoc_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/common_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/common_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/feedparser_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/feedparser_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/feedparser_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/feedparser_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/news_sdk_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/news_sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/newsapi_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/newsapi_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/newsapi_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/newsapi_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/qa_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/qa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/qa_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/qa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/rolling_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/rolling_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/quantitative_analysis/rolling_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/quantitative_analysis/rolling_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/custom_indicators_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/custom_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/custom_indicators_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/custom_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/momentum_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/momentum_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/momentum_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/momentum_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/overlap_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/overlap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/overlap_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/overlap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/ta_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/trend_indicators_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/trend_indicators_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/trend_indicators_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/trend_indicators_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volatility_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volatility_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volatility_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volatility_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volume_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volume_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/technical_analysis/volume_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/technical_analysis/volume_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/ultima_newsmonitor_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/ultima_newsmonitor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/common/ultima_newsmonitor_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/common/ultima_newsmonitor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/config_terminal.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/config_terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/completer/choices.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/completer/choices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/config/paths.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/config/paths.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/config/paths_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/config/paths_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/README.md` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/controllers.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/controllers.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/integration_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/integration_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/integration_test_coverage.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/integration_test_coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/integration_tests/utils.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/integration_tests/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/log_sender.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/log_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/logging_clock.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/logging_clock.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/collection/s3_sender.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/collection/s3_sender.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/common.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/common.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/custom_logger.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/custom_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/directories.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/directories.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/expired_files.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/formatter_with_exceptions.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/path_tracking_file_handler.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/settings.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/log/generation/settings_logger.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/log/generation/settings_logger.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/__init__.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/base_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/base_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/credentials_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/credentials_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/preferences_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/preferences_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/profile_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/profile_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/sources_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/sources_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/system_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/system_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/models/user_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/models/user_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/assets/Terminal_icon.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/backend.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/config/openbb_styles.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/no_import.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/no_import.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly.html` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/base.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/data_classes.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/plotly_ta/ta_class.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/plots/table.html` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/plots/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/scripts/sdk_audit.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/scripts/sdk_audit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/alt_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/crypto_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/etf_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/forex_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/portfolio_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/controllers/stocks_sdk_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/__init__.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/alt_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/alt_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/crypto_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/crypto_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/econometrics_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/econometrics_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/economy_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/economy_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/etf_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/etf_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/fixedincome_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/forecast_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/forecast_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/forex_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/forex_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/funds_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/funds_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/futures_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/futures_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/keys_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/keys_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/portfolio_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/portfolio_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/qa_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/qa_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/stocks_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/stocks_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/models/ta_sdk_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/models/ta_sdk_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/sdk_init.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/sdk_init.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map_forecasting.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map_forecasting.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trail_map_optimization.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trail_map_optimization.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sdk/trailmap.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sdk/trailmap.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/banner.txt` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/banner.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/constants.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/current_system.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/current_system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/current_user.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/current_user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/env_handler.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/env_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/hub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/hub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/local_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/local_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/routines_handler.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/routines_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/sdk_session.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/sdk_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/session_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/session_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/session_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/session_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/sources_handler.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/sources_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/session/utils.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/session/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/core/sources/utils.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/core/sources/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/coinbase_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/coinbase_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/coinpaprika_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/coinpaprika_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_models.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/crypto_views.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/crypto_views.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/cryptocurrency_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/README.md` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/binance_gecko_map.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/binance_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coinbase_gecko_map.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coingecko_categories.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coingecko_categories.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coingecko_coins.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coingecko_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/coinpaprika_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/defillama_dapps.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/defillama_dapps.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/erc20_coins.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/erc20_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/finbrain_coins.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/finbrain_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/santiment_slugs.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/santiment_slugs.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/data/yahoofinance_coins.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/dataframe_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/dataframe_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/coindix_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/coindix_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/coindix_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/coindix_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/cryptosaurio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/cryptosaurio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/defi_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/defi_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/graph_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/graph_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/graph_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/graph_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/llama_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/llama_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/llama_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/llama_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/smartstake_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/smartstake_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/smartstake_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/smartstake_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/substack_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/substack_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/substack_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/substack_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terraengineer_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terraengineer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terraengineer_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terraengineer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terramoney_fcd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/defi/terramoney_fcd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinmarketcap_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinmarketcap_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/dappradar_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/dappradar_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/dappradar_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/dappradar_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/discovery_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/discovery/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/binance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/binance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/binance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/binance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/ccxt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/ccxt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinglass_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinglass_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/dd_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/due_diligence_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/finbrain_crypto_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/messari_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/messari_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/messari_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/messari_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/santiment_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/santiment_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/due_diligence/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nft_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nft_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nftpricefloor_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/nftpricefloor_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/opensea_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/opensea_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/nft/opensea_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/nft/opensea_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/bitquery_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/bitquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/bitquery_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/bitquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/blockchain_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/blockchain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/blockchain_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/blockchain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethgasstation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethgasstation_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethplorer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/ethplorer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/onchain_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/onchain_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/shroom_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/shroom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/shroom_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/shroom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/whale_alert_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/onchain/whale_alert_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/blockchaincenter_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/blockchaincenter_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinbase_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinbase_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinpaprika_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/coinpaprika_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/cryptopanic_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/cryptopanic_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/glassnode_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/glassnode_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/glassnode_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/glassnode_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/loanscan_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/loanscan_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/loanscan_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/loanscan_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/overview_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/overview_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/pycoingecko_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/pycoingecko_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/rekt_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/rekt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/rekt_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/rekt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/tokenterminal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/tokenterminal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/withdrawalfees_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/overview/withdrawalfees_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pycoingecko_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pycoingecko_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pyth_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pyth_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/pyth_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/pyth_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/cryptocurrency/tools/tools_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/cryptocurrency/tools/tools_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_prompt_toolkit.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_prompt_toolkit.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/coin_highs.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/coin_highs.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_crash.html` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_crash.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_supply.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_supply.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/luna_terra.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/luna_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/lunatics.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/tvl.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/tvl.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/custom_reports/lunar_crash/ust_terra.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/custom_reports/lunar_crash/ust_terra.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/dashboards_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/dashboards_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/Forecasting.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/Forecasting.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/common_vars.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/common_vars.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Chains.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Correlation.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Correlation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Futures.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Futures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Indicators.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Short_Data.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Short_Data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/pages/Stocks.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/pages/Stocks.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/stream/streamlit_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/stream/streamlit_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/streamlit_run.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/streamlit_run.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/chains.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/chains.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/correlation.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/correlation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/forecast.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/futures.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/futures.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/shortdata.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/shortdata.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/dashboards/voila/stocks.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/dashboards/voila/stocks.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/decorators.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/econometrics_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/econometrics_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/regression_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/regression_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/econometrics/regression_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/econometrics/regression_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/alphavantage_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/alphavantage_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/alphavantage_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/alphavantage_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/commodity_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/commodity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/commodity_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/commodity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/NASDAQ_CountryCodes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/cpi.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/datasets/harmonized_cpi.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/datasets/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/econdb_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/econdb_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/economy_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/economy_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/economy_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/economy_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/finviz_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/finviz_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/fred_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/fred_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/nasdaq_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/nasdaq_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/oecd_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/oecd_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/plot_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/plot_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/wsj_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/wsj_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/yfinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/economy/yfinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/economy/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/disc_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/wsj_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/wsj_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/discovery/wsj_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/discovery/wsj_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/etf_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/etf_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/etfs.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/etfs.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/financedatabase_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/financedatabase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/financedatabase_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/financedatabase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/fmp_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/fmp_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/stockanalysis_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/stockanalysis_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/stockanalysis_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/stockanalysis_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/etf/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/etf/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/featflags_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/featflags_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/commercial_paper.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/corporate_spot_rates.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ecb_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ecb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ecb_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ecb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/econdb_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/econdb_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/econdb_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/econdb_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fixedincome_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fixedincome_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fred_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/fred_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/fred_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/ice_bofa_indices.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/oecd_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/oecd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/oecd_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/oecd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/yfinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/fixedincome/yfinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/fixedincome/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/anom_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/anom_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/anom_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/anom_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoarima_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoarima_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoarima_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoarima_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoces_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoces_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoces_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoces_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoets_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoets_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoets_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoets_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoselect_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoselect_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/autoselect_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/autoselect_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/brnn_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/brnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/brnn_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/brnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/expo_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/expo_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/expo_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/expo_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/forecast_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/forecast_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/linregr_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/linregr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/linregr_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/linregr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/mstl_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/mstl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/mstl_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/mstl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nbeats_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nbeats_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nbeats_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nbeats_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nhits_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nhits_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/nhits_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/nhits_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/regr_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/regr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/regr_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/regr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rnn_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rnn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rnn_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rnn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rwd_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rwd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/rwd_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/rwd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/seasonalnaive_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/seasonalnaive_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/seasonalnaive_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/seasonalnaive_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tcn_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tcn_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tcn_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tcn_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tft_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tft_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/tft_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/tft_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/theta_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/theta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/theta_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/theta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/trans_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/trans_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/trans_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/trans_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/whisper_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/whisper_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forecast/whisper_utils.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forecast/whisper_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/av_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/av_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/av_forex_currencies.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/av_forex_currencies.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/polygon_tickers.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/polygon_tickers.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/data/yahoofinance_forex.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/data/yahoofinance_forex.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/forex_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/forex_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/forex_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/forex_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/fxempire_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/fxempire_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/fxempire_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/fxempire_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/oanda/oanda_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/oanda/oanda_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/polygon_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/forex/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/forex/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/databento_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/databento_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/futures_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/futures_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/sdk_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/yfinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/futures/yfinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/futures/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/helper_classes.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/helper_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/helper_funcs.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/helper_funcs.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/helpers_denomination.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/helpers_denomination.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/intro.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/intro.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -310,25 +310,23 @@
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if (
         current_user.credentials.API_KEY_ALPHAVANTAGE == "REPLACE_ME"
     ):  # pragma: allowlist secret
-        logger.info("Alpha Vantage key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         df = TimeSeries(
             key=current_user.credentials.API_KEY_ALPHAVANTAGE, output_format="pandas"
         ).get_intraday(symbol="AAPL")
         if df[0].empty:  # pylint: disable=no-member
             logger.warning("Alpha Vantage key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         else:
-            logger.info("Alpha Vantage key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -380,26 +378,24 @@
 
     current_user = get_current_user()
 
     if (
         current_user.credentials.API_KEY_FINANCIALMODELINGPREP
         == "REPLACE_ME"  # pragma: allowlist secret
     ):  # pragma: allowlist secret
-        logger.info("Financial Modeling Prep key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             f"https://financialmodelingprep.com/api/v3/profile/AAPL?apikey="
             f"{current_user.credentials.API_KEY_FINANCIALMODELINGPREP}"
         )
         if r.status_code in [403, 401] or "Error Message" in str(r.content):
             logger.warning("Financial Modeling Prep key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Financial Modeling Prep key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Financial Modeling Prep key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -454,21 +450,19 @@
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if (
         current_user.credentials.API_KEY_QUANDL == "REPLACE_ME"
     ):  # pragma: allowlist secret
-        logger.info("Quandl key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         try:
             quandl.save_key(current_user.credentials.API_KEY_QUANDL)
             quandl.get("EIA/PET_RWTC_D")
-            logger.info("Quandl key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         except Exception as _:  # noqa: F841
             logger.warning("Quandl key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -521,27 +515,25 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_POLYGON_KEY == "REPLACE_ME":
-        logger.info("Polygon key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         check_date = date(date.today().year, date.today().month, 1).isoformat()
         r = request(
             f"https://api.polygon.io/v2/aggs/ticker/AAPL/range/1/day/{check_date}"
             f"/{check_date}?apiKey={current_user.credentials.API_POLYGON_KEY}"
         )
         if r.status_code in [403, 401]:
             logger.warning("Polygon key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Polygon key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Polygon key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -594,25 +586,23 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_FRED_KEY == "REPLACE_ME":
-        logger.info("FRED key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             f"https://api.stlouisfed.org/fred/series?series_id=GNPCA&api_key={current_user.credentials.API_FRED_KEY}"
         )
         if r.status_code in [403, 401, 400]:
             logger.warning("FRED key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("FRED key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("FRED key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -665,25 +655,23 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_NEWS_TOKEN == "REPLACE_ME":  # nosec
-        logger.info("News API key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             f"https://newsapi.org/v2/everything?q=keyword&apiKey={current_user.credentials.API_NEWS_TOKEN}"
         )
         if r.status_code in [401, 403]:
             logger.warning("News API key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("News API key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("News API key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -736,29 +724,27 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_BIZTOC_TOKEN == "REPLACE_ME":  # nosec
-        logger.info("BizToc API key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://biztoc.p.rapidapi.com/pages",
             headers={
                 "X-RapidAPI-Key": current_user.credentials.API_BIZTOC_TOKEN,
                 "X-RapidAPI-Host": "biztoc.p.rapidapi.com",
             },
         )
         if r.status_code in [401, 403, 404]:
             logger.warning("BizToc API key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("BizToc API key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("BizToc API key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -811,30 +797,28 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_TRADIER_TOKEN == "REPLACE_ME":  # nosec
-        logger.info("Tradier key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://sandbox.tradier.com/v1/markets/quotes",
             params={"symbols": "AAPL"},
             headers={
                 "Authorization": f"Bearer {current_user.credentials.API_TRADIER_TOKEN}",
                 "Accept": "application/json",
             },
         )
         if r.status_code in [401, 403]:
             logger.warning("Tradier key not defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Tradier key not defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Tradier key not defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -886,25 +870,22 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_CMC_KEY == "REPLACE_ME":
-        logger.info("Coinmarketcap key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         cmc = CoinMarketCapAPI(current_user.credentials.API_CMC_KEY)
 
         try:
             cmc.cryptocurrency_map()
-            logger.info("Coinmarketcap key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         except Exception:
-            logger.info("Coinmarketcap key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -954,25 +935,23 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_FINNHUB_KEY == "REPLACE_ME":
-        logger.info("Finnhub key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = r = request(
             f"https://finnhub.io/api/v1/quote?symbol=AAPL&token={current_user.credentials.API_FINNHUB_KEY}"
         )
         if r.status_code in [403, 401, 400]:
             logger.warning("Finnhub key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Finnhub key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Finnhub key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -1059,15 +1038,14 @@
         current_user.credentials.API_REDDIT_CLIENT_ID,
         current_user.credentials.API_REDDIT_CLIENT_SECRET,
         current_user.credentials.API_REDDIT_USERNAME,
         current_user.credentials.API_REDDIT_PASSWORD,
         current_user.credentials.API_REDDIT_USER_AGENT,
     ]
     if "REPLACE_ME" in reddit_keys:
-        logger.info("Reddit key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         try:
             with suppress_stdout():
                 praw_api = praw.Reddit(
                     client_id=current_user.credentials.API_REDDIT_CLIENT_ID,
                     client_secret=current_user.credentials.API_REDDIT_CLIENT_SECRET,
@@ -1085,15 +1063,14 @@
                     reddit_url="https://www.reddit.com",
                     short_url="https://redd.it",
                     ratelimit_seconds=5,
                     timeout=16,
                 )
 
                 praw_api.user.me()
-            logger.info("Reddit key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         except (Exception, ResponseException):
             logger.warning("Reddit key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -1148,15 +1125,14 @@
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     bitquery = current_user.credentials.API_BITQUERY_KEY
     if "REPLACE_ME" in bitquery:
-        logger.info("Bitquery key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         headers = {"x-api-key": current_user.credentials.API_BITQUERY_KEY}
         query = """
         {
         ethereum {
         dexTrades(options: {limit: 10, desc: "count"}) {
@@ -1167,15 +1143,14 @@
         r = request(
             "https://graphql.bitquery.io",
             method="POST",
             json={"query": query},
             headers=headers,
         )
         if r.status_code == 200:
-            logger.info("Bitquery key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Bitquery key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -1243,15 +1218,14 @@
     """
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
     if current_user.credentials.API_TWITTER_BEARER_TOKEN == "REPLACE_ME":
-        logger.info("Twitter key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         params = {
             "query": "(\\$AAPL) (lang:en)",
             "max_results": "10",
             "tweet.fields": "created_at,lang",
         }
@@ -1260,15 +1234,14 @@
             params=params,  # type: ignore
             headers={
                 "authorization": "Bearer "
                 + current_user.credentials.API_TWITTER_BEARER_TOKEN
             },
         )
         if r.status_code == 200:
-            logger.info("Twitter key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         elif r.status_code in [401, 403]:
             logger.warning("Twitter key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         else:
             logger.warning("Twitter key defined, test failed")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
@@ -1338,20 +1311,19 @@
 
     current_user = get_current_user()
 
     rh_keys = [
         current_user.credentials.RH_USERNAME,
         current_user.credentials.RH_PASSWORD,
     ]
-    if "REPLACE_ME" in rh_keys:
-        logger.info("Robinhood key not defined")
-        status = KeyStatus.NOT_DEFINED
-    else:
-        logger.info("Robinhood key defined, not tested")
-        status = KeyStatus.DEFINED_NOT_TESTED
+    status = (
+        KeyStatus.NOT_DEFINED
+        if "REPLACE_ME" in rh_keys
+        else KeyStatus.DEFINED_NOT_TESTED
+    )
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
 
@@ -1421,34 +1393,30 @@
 
     dg_keys = [
         current_user.credentials.DG_USERNAME,
         current_user.credentials.DG_PASSWORD,
         current_user.credentials.DG_TOTP_SECRET,
     ]
     if "REPLACE_ME" in dg_keys:
-        logger.info("Degiro key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         dg = DegiroModel()
         try:
             f = io.StringIO()  # suppress stdout
             with contextlib.redirect_stdout(f):
                 check_creds = dg.check_credentials()  # pylint: disable=no-member
 
             if "2FA is enabled" in f.getvalue() or check_creds:
-                logger.info("Degiro key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
             else:
                 raise Exception
 
-            logger.info("Degiro key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
 
         except Exception:
-            logger.info("Degiro key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
         del dg  # ensure the object is destroyed explicitly
 
     if show_output:
         console.print(status.colorize())
 
@@ -1521,30 +1489,27 @@
     current_user = get_current_user()
 
     oanda_keys = [
         current_user.credentials.OANDA_TOKEN,
         current_user.credentials.OANDA_ACCOUNT,
     ]
     if "REPLACE_ME" in oanda_keys:
-        logger.info("Oanda key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         client = oanda_API(access_token=current_user.credentials.OANDA_TOKEN)
         account = current_user.credentials.OANDA_ACCOUNT
         try:
             parameters = {"instruments": "EUR_USD"}
             request_ = oandapyV20.endpoints.pricing.PricingInfo(
                 accountID=account, params=parameters
             )
             client.request(request_)
-            logger.info("Oanda key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
 
         except Exception:
-            logger.info("Oanda key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -1609,25 +1574,23 @@
 
     current_user = get_current_user()
 
     if "REPLACE_ME" in [
         current_user.credentials.API_BINANCE_KEY,
         current_user.credentials.API_BINANCE_SECRET,
     ]:
-        logger.info("Binance key not defined")
         status = KeyStatus.NOT_DEFINED
 
     else:
         try:
             client = binance.Client(
                 current_user.credentials.API_BINANCE_KEY,
                 current_user.credentials.API_BINANCE_SECRET,
             )
             client.get_account_api_permissions()
-            logger.info("Binance key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         except Exception:
             logger.warning("Binance key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -1700,15 +1663,14 @@
     current_user = get_current_user()
 
     if "REPLACE_ME" in [
         current_user.credentials.API_COINBASE_KEY,
         current_user.credentials.API_COINBASE_SECRET,
         current_user.credentials.API_COINBASE_PASS_PHRASE,
     ]:
-        logger.info("Coinbase key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         auth = CoinbaseProAuth(
             current_user.credentials.API_COINBASE_KEY,
             current_user.credentials.API_COINBASE_SECRET,
             current_user.credentials.API_COINBASE_PASS_PHRASE,
         )
@@ -1716,15 +1678,14 @@
             resp = make_coinbase_request("/accounts", auth=auth)
         except CoinbaseApiException:
             resp = None
         if not resp:
             logger.warning("Coinbase key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         else:
-            logger.info("Coinbase key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -1774,31 +1735,28 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_WHALE_ALERT_KEY == "REPLACE_ME":
-        logger.info("Walert key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         url = (
             "https://api.whale-alert.io/v1/transactions?api_key="
             + current_user.credentials.API_WHALE_ALERT_KEY
         )
         try:
             response = request(url)
             if not 200 <= response.status_code < 300:
                 logger.warning("Walert key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
             else:
-                logger.info("Walert key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
         except Exception:
-            logger.info("Walert key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -1850,30 +1808,28 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_GLASSNODE_KEY == "REPLACE_ME":
-        logger.info("Glassnode key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         url = "https://api.glassnode.com/v1/metrics/market/price_usd_close"
 
         parameters = {
             "api_key": current_user.credentials.API_GLASSNODE_KEY,
             "a": "BTC",
             "i": "24h",
             "s": str(1_614_556_800),
             "u": str(1_641_227_783_561),
         }
 
         r = request(url, params=parameters)
         if r.status_code == 200:
-            logger.info("Glassnode key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Glassnode key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -1928,28 +1884,26 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_COINGLASS_KEY == "REPLACE_ME":
-        logger.info("Coinglass key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         url = "https://open-api.coinglass.com/api/pro/v1/futures/openInterest/chart?&symbol=BTC&interval=0"
 
         headers = {"coinglassSecret": current_user.credentials.API_COINGLASS_KEY}
 
         response = request(url, headers=headers)
 
         if """success":false""" in str(response.content):
             logger.warning("Coinglass key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif response.status_code == 200:
-            logger.info("Coinglass key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Coinglass key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -2002,25 +1956,23 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_CRYPTO_PANIC_KEY == "REPLACE_ME":
-        logger.info("cpanic key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         crypto_panic_url = (
             "https://cryptopanic.com/api/v1/posts/?auth_token="
             f"{current_user.credentials.API_CRYPTO_PANIC_KEY}"
         )
         response = request(crypto_panic_url)
 
         if response.status_code == 200:
-            logger.info("Cpanic key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Cpanic key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -2075,30 +2027,27 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_ETHPLORER_KEY == "REPLACE_ME":
-        logger.info("ethplorer key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         ethplorer_url = "https://api.ethplorer.io/getTokenInfo/0x1f9840a85d5af5bf1d1762f925bdaddc4201f984?apiKey="
         ethplorer_url += current_user.credentials.API_ETHPLORER_KEY
 
         try:
             response = request(ethplorer_url)
             if response.status_code == 200:
-                logger.info("ethplorer key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
             else:
                 logger.warning("ethplorer key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
         except Exception as _:  # noqa: F841
-            logger.info("ethplorer key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -2180,15 +2129,14 @@
                 "errors" in str(response.content)
                 or response.status_code < 200
                 or response.status_code >= 300
             ):
                 logger.warning("Smartstake key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
             elif 200 <= response.status_code < 300:
-                logger.info("Smartstake key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
             else:
                 logger.warning("Smartstake key defined, test inconclusive")
                 status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
         except Exception as _:  # noqa: F841
             logger.warning("Smartstake key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
@@ -2246,15 +2194,14 @@
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if (
         current_user.credentials.API_GITHUB_KEY == "REPLACE_ME"
     ):  # pragma: allowlist secret
-        logger.info("GitHub key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         status = KeyStatus.DEFINED_NOT_TESTED
         # github api will not fail for the first requests without key
         # only after certain amount of requests the user will get rate limited
 
     if show_output:
@@ -2311,24 +2258,22 @@
 
     current_user = get_current_user()
 
     if (
         current_user.credentials.API_MESSARI_KEY
         == "REPLACE_ME"  # pragma: allowlist secret
     ):  # pragma: allowlist secret
-        logger.info("Messari key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         url = "https://data.messari.io/api/v2/assets/bitcoin/profile"
         headers = {"x-messari-api-key": current_user.credentials.API_MESSARI_KEY}
         params = {"fields": "profile/general/overview/official_links"}
         r = request(url, headers=headers, params=params)
 
         if r.status_code == 200:
-            logger.info("Messari key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Messari key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -2381,24 +2326,22 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_EODHD_KEY == "REPLACE_ME":  # nosec
-        logger.info("End of Day Historical Data key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         request_url = (
             "https://eodhistoricaldata.com/api/exchanges-list/?api_token="
             f"{current_user.credentials.API_EODHD_KEY}&fmt=json"
         )
         r = request(request_url)
         if r.status_code == 200:
-            logger.info("Eodhd key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Eodhd key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -2453,15 +2396,14 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_SANTIMENT_KEY == "REPLACE_ME":
-        logger.info("santiment key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         headers = {
             "Content-Type": "application/graphql",
             "Authorization": f"Apikey {current_user.credentials.API_SANTIMENT_KEY}",
         }
 
@@ -2472,21 +2414,19 @@
             "https://api.santiment.net/graphql",
             method="POST",
             headers=headers,
             data=data,
         )
         try:
             if response.status_code == 200:
-                logger.info("santiment key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
             else:
                 logger.warning("santiment key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
         except Exception as _:  # noqa: F841
-            logger.info("santiment key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -2536,26 +2476,24 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_SHROOM_KEY == "REPLACE_ME":
-        logger.info("Shroom key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         try:
             response = request(
                 "https://node-api.flipsidecrypto.com/queries",
                 method="POST",
                 headers={"x-api-key": current_user.credentials.API_SHROOM_KEY},
             )
             if response.status_code == 400:
                 # this is expected because shroom returns 400 when query is not passed
-                logger.info("Shroom key defined, test passed")
                 status = KeyStatus.DEFINED_TEST_PASSED
             elif response.status_code == 401:
                 logger.warning("Shroom key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
             else:
                 logger.warning("Shroom key defined, test failed")
                 status = KeyStatus.DEFINED_TEST_FAILED
@@ -2614,26 +2552,24 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_TOKEN_TERMINAL_KEY == "REPLACE_ME":
-        logger.info("Token Terminal key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         token_terminal = TokenTerminal(
             key=current_user.credentials.API_TOKEN_TERMINAL_KEY
         )
 
         if "message" in token_terminal.get_all_projects():
             logger.warning("Token Terminal key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         else:
-            logger.info("Token Terminal key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
 
     if show_output:
         console.print(status.colorize())
 
     return str(status)
 
@@ -2682,22 +2618,20 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_STOCKSERA_KEY == "REPLACE_ME":
-        logger.info("Stocksera key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         client = stocksera.Client(api_key=current_user.credentials.API_STOCKSERA_KEY)
 
         try:
             client.borrowed_shares(ticker="AAPL")
-            logger.info("Stocksera key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         except Exception as _:  # noqa: F841
             logger.warning("Stocksera key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
 
     if show_output:
         console.print(status.colorize())
@@ -2749,25 +2683,23 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_INTRINIO_KEY == "REPLACE_ME":
-        logger.info("Intrinio key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             f"https://api-v2.intrinio.com/securities/AAPL/prices?api_key={current_user.credentials.API_INTRINIO_KEY}"
         )
         if r.status_code in [403, 401, 429]:
             logger.warning("Intrinio key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Intrinio key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Intrinio key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -2822,26 +2754,24 @@
 
     if show_output:
         console.print("Checking status...")
 
     current_user = get_current_user()
 
     if current_user.credentials.API_DATABENTO_KEY == "REPLACE_ME":
-        logger.info("DataBento key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://hist.databento.com/v0/metadata.list_datasets",
             auth=(f"{current_user.credentials.API_DATABENTO_KEY}", ""),
         )
         if r.status_code in [403, 401, 429]:
             logger.warning("DataBento key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("DataBento key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("DataBento key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -2891,28 +2821,26 @@
     str
         Status of key set
     """
 
     current_user = get_current_user()
 
     if current_user.credentials.API_ULTIMA_KEY == "REPLACE_ME":
-        logger.info("Ultima Insights key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://api.ultimainsights.ai/v1/checkAPIKey",
             headers={
                 "Authorization": f"Bearer {current_user.credentials.API_ULTIMA_KEY}"
             },
         )
         if r.status_code in [403, 401, 429]:
             logger.warning("Ultima Insights key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("Ultima Insights key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("Ultima Insights key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
@@ -2964,26 +2892,24 @@
     str
         Status of key set
     """
 
     current_user = get_current_user()
 
     if current_user.credentials.API_DAPPRADAR_KEY == "REPLACE_ME":
-        logger.info("DappRadar key not defined")
         status = KeyStatus.NOT_DEFINED
     else:
         r = request(
             "https://api.dappradar.com/4tsxo4vuhotaojtl/tokens/chains",
             headers={"X-BLOBR-KEY": current_user.credentials.API_DAPPRADAR_KEY},
         )
         if r.status_code in [403, 401, 429]:
             logger.warning("DappRadar key defined, test failed")
             status = KeyStatus.DEFINED_TEST_FAILED
         elif r.status_code == 200:
-            logger.info("DappRadar key defined, test passed")
             status = KeyStatus.DEFINED_TEST_PASSED
         else:
             logger.warning("DappRadar key defined, test inconclusive")
             status = KeyStatus.DEFINED_TEST_INCONCLUSIVE
 
     if show_output:
         console.print(status.colorize())
```

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/keys_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/keys_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/loggers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/loggers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/menu.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/menu.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/documentation_commands_sdk.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/documentation_scripts/generate_documentation_commands.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/documentation_scripts/generate_documentation_commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/futures/futures.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/futures/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/i18n/en.yml` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/i18n/en.yml`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/i18n/help_translation.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/i18n/help_translation.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/README.MD`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_crypto.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_dd.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_dd.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_defi.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_defi.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_discovery.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_discovery.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_onchain.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_onchain.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_overview.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_overview.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_qa.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_ta.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/cryptocurrency/test_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/econometrics/test_econometrics.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/economy/test_economy.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ta.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/etf/test_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/fixedincome/test_fixedincome.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forecast/test_forecast.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_oanda.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_oanda.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_qa.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_ta.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/forex/test_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_po.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/portfolio/test_portfolio.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_bt.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_bt.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ca.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ca.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_fa.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_fa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_qa.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_qa.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_stocks.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ta.openbb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/integration_tests_scripts/stocks/test_ta.openbb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/models/hub_credentials.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/models/hub_credentials.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/allocation_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/holdings_example.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/portfolio/parameters_template.xlsx` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/portfolio/parameters_template.xlsx`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/sources/openbb_default.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/sources/openbb_default.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Agriculture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Agro-Chemicals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Air-Transportation.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Apparel.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Banks.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Banks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Brokers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Building-Materials.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Business-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Closed-End-Funds.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Construction.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Construction.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Credit-Industry.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Durable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Electronics.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Furniture.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Gold-Silver.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Grocery.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Ground-Freight.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Guided-Missiles.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Health.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Health.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Hotels.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Insurance-Agents.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Insurance-Carriers.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Investment-Offices.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Legal.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Legal.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Lumber.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Manufacturing.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Mining.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Mining.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Mortgages.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Nondurable-Goods.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Personal-Credit.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Pharmaceuticals.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Professional-Services.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Railroads.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Real-Estate.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Restaurants.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Retail-Stores.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Retail-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Tobacco.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Utility-Communications.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Utility-Gas.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/Wholesale-Trade.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/template.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/template.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/insider/whales.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/insider/whales.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/all_parameters.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/growth_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/stocks/screener/value_stocks.ini`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/Consolas.ttf` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/Consolas.ttf`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.mplstyle` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.mpfstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.mplstyle` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.mplstyle`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/miscellaneous/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_fund_ID.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_fund_ID.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/avanza_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/avanza_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mstarpy_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mstarpy_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mstarpy_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mstarpy_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mutual_fund_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mutual_fund_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/mutual_funds/mutual_funds_utils.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/mutual_funds/mutual_funds_utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/parent_classes.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/parent_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/allocation_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/allocation_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/attribution_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/attribution_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/bro_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/bro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/brokers_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/brokers_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/coinbase/coinbase_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/README.md` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/degiro/degiro_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/degiro/degiro_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/brokers/robinhood/robinhood_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/metrics_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/metrics_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_engine.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/excel_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/excel_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/optimizer_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/Parameter.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/parameters/params_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_engine.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_engine.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/po_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/po_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/statics.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_optimization/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/portfolio_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/portfolio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/portfolio/statics.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/portfolio/statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/.ipynb_checkpoints/test-checkpoint.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/README.md` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/reports_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/reports_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/reports_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/reports_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/stored/20220512_040312_equity_NVDA.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/OpenBB_reports_logo.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/OpenBB_reports_logo.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/crypto.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/crypto.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/economy.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/economy.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/equity.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/equity.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/etf.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/etf.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/floppy-disc.png` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/floppy-disc.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/forecast.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/forecast.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/forex.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/forex.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/templates/portfolio.ipynb` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/templates/portfolio.ipynb`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widget_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widget_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/report.css` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/report.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/reports/widgets/style.css` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/reports/widgets/style.css`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/rich_config.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/rich_config.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/routine_functions.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/routine_functions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/sdk.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/sdk.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/settings_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/settings_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/sources_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/sources_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/backtesting/bt_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/backtesting/bt_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/ba_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/ba_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/behavioural_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/cboe_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/cboe_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/cboe_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/cboe_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/ca_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/ca_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finbrain_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finbrain_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finnhub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finviz_compare_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/finviz_compare_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/polygon_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/comparison_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/dps_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/finra_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/finra_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/finra_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/finra_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/ibkr_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/ibkr_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/quandl_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/quandl_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/sec_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/sec_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/sec_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/sec_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stockgrid_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stockgrid_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stocksera_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/stocksera_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/dark_pool_shorts/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/databento_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/databento_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/ark_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/ark_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/ark_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/ark_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/disc_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/disc_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fidelity_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fidelity_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fidelity_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fidelity_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finnhub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finnhub_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finviz_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/finviz_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/fmp_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/nasdaq_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/nasdaq_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/seeking_alpha_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/seeking_alpha_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/shortinterest_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/shortinterest_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/shortinterest_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/shortinterest_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/yahoofinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/yahoofinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/discovery/yahoofinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/discovery/yahoofinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/av_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/av_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/av_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/av_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/business_insider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/business_insider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/csimarket_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/csimarket_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_static.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_static.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/dcf_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/dcf_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eclect_us_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eclect_us_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eodhd_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/eodhd_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fa_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finnhub_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finnhub_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finviz_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/finviz_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fmp_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fmp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/fmp_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/fmp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/key_metrics_explained.txt`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/marketwatch_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/marketwatch_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/nasdaq_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/nasdaq_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/nasdaq_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/polygon_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/polygon_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/polygon_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/polygon_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/sdk_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/seeking_alpha_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/fundamental_analysis/yahoo_finance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/gov_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/gov_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/quiverquant_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/quiverquant_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/government/quiverquant_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/government/quiverquant_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/businessinsider_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/businessinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/businessinsider_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/businessinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/finviz_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/finviz_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/insider_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/insider_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/openinsider_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/openinsider_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/openinsider_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/openinsider_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/insider/sdk_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/insider/sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/mappings/Mic_Codes.csv` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/mappings/Mic_Codes.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/alphaquery_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/alphaquery_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/alphaquery_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/alphaquery_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/barchart_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/barchart_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/barchart_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/barchart_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/calculator_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/calculator_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/calculator_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/calculator_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/chartexchange_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/chartexchange_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/chartexchange_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/chartexchange_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/fdscanner_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/fdscanner_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/fdscanner_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/fdscanner_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/hedge/hedge_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/hedge/hedge_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/intrinio_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/intrinio_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/intrinio_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/intrinio_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/nasdaq_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/nasdaq_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/op_helpers.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/op_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_sdk_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_sdk_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/options_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/options_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/tradier_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/tradier_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/tradier_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/tradier_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/yfinance_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/yfinance_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/options/yfinance_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/options/yfinance_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/beta_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/beta_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/beta_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/beta_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/factors_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/factors_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/factors_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/factors_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/quantitative_analysis/qa_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/quantitative_analysis/qa_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/research/res_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/research/res_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/finviz_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/finviz_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/finviz_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/finviz_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/screener/screener_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/screener/screener_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stock_statics.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stock_statics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/stocks_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/stocks_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/finbrain_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/finbrain_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/finbrain_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/finbrain_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/rsp_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/rsp_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/rsp_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/rsp_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/ta_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/ta_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/tradingview_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/tradingview_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/technical_analysis/tradingview_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/technical_analysis/tradingview_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/bursa_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/bursa_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/bursa_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/bursa_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/data/bursa_open_hours.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/pandas_market_cal_model.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/pandas_market_cal_view.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/tradinghours_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/tradinghours_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/stocks/tradinghours/tradinghours_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/stocks/tradinghours/tradinghours_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/terminal_controller.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/terminal_controller.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/terminal_helper.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/terminal_helper.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/openbb_terminal/thought_of_the_day.py` & `openbb_nightly-3.0.1.dev20230608/openbb_terminal/thought_of_the_day.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/pyproject.toml` & `openbb_nightly-3.0.1.dev20230608/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbb-nightly"
-version = "3.0.1.dev20230607"
+version = "3.0.1.dev20230608"
 description = "Investment Research for Everyone, Anywhere."
 license = "MIT"
 authors = ["Didier Rodrigues Lopes"]
 packages = [
     { include = "openbb_terminal" },
 ]
 include = ["terminal.py", "openbb_terminal/.env"]
```

### Comparing `openbb_nightly-3.0.1.dev20230607/terminal.py` & `openbb_nightly-3.0.1.dev20230608/terminal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/website/pypi.md` & `openbb_nightly-3.0.1.dev20230608/website/pypi.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-3.0.1.dev20230607/PKG-INFO` & `openbb_nightly-3.0.1.dev20230608/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 3.0.1.dev20230607
+Version: 3.0.1.dev20230608
 Summary: Investment Research for Everyone, Anywhere.
 Home-page: https://openbb.co
 License: MIT
 Author: Didier Rodrigues Lopes
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

