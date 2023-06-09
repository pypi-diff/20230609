# Comparing `tmp/OctoBot-0.4.8.tar.gz` & `tmp/OctoBot-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OctoBot-0.4.8.tar", last modified: Sun Sep  4 12:12:18 2022, max compression
+gzip compressed data, was "OctoBot-0.4.9.tar", last modified: Wed Sep  7 23:12:40 2022, max compression
```

## Comparing `OctoBot-0.4.8.tar` & `OctoBot-0.4.9.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.895619 OctoBot-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)    51143 2022-09-04 12:11:04.000000 OctoBot-0.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-09-04 12:11:04.000000 OctoBot-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-04 12:11:04.000000 OctoBot-0.4.8/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.831618 OctoBot-0.4.8/OctoBot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-04 12:12:18.000000 OctoBot-0.4.8/OctoBot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-09-04 12:12:18.895619 OctoBot-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8236 2022-09-04 12:11:04.000000 OctoBot-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.835619 OctoBot-0.4.8/octobot/
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.835619 OctoBot-0.4.8/octobot/api/
--rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4434 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/api/backtesting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5259 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/api/strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/api/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.835619 OctoBot-0.4.8/octobot/backtesting/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/abstract_backtesting_test.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/abstract_backtesting_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/independent_backtesting.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    22103 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/independent_backtesting.py
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/octobot_backtesting.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/backtesting/octobot_backtesting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.835619 OctoBot-0.4.8/octobot/channels/
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/channels/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/channels/octobot_channel.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/channels/octobot_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)    19570 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7573 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.839619 OctoBot-0.4.8/octobot/community/
--rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22985 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     7359 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_donation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_supports.py
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_tentacles_package.py
--rw-r--r--   0 runner    (1001) docker     (121)     3040 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/community_user_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.839619 OctoBot-0.4.8/octobot/community/errors_upload/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/errors_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/errors_upload/error_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/errors_upload/errors_uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/errors_upload/initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.839619 OctoBot-0.4.8/octobot/community/feeds/
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/feeds/abstract_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)    13187 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/feeds/community_mqtt_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)    11239 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/feeds/community_ws_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/feeds/feed_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/graphql_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/community/identifiers_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.839619 OctoBot-0.4.8/octobot/config/
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/config/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/config/default_config.json
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/config/logging_config.ini
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/config/profile_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/configuration_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10569 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7805 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/disclaimer.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/initializer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/initializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    15341 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_api.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_backtesting_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_backtesting_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_channel_consumer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6014 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/octobot_channel_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.839619 OctoBot-0.4.8/octobot/producers/
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/evaluator_producer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/evaluator_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/exchange_producer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/exchange_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/interface_producer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9203 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/interface_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/service_feed_producer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/producers/service_feed_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.843618 OctoBot-0.4.8/octobot/strategy_optimizer/
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.883619 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/
--rw-r--r--   0 runner    (1001) docker     (121)   950272 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data
--rw-r--r--   0 runner    (1001) docker     (121)   937984 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data
--rw-r--r--   0 runner    (1001) docker     (121)   942080 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data
--rw-r--r--   0 runner    (1001) docker     (121)   958464 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data
--rw-r--r--   0 runner    (1001) docker     (121)   876544 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data
--rw-r--r--   0 runner    (1001) docker     (121)   978944 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data
--rw-r--r--   0 runner    (1001) docker     (121)   946176 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data
--rw-r--r--   0 runner    (1001) docker     (121)   913408 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data
--rw-r--r--   0 runner    (1001) docker     (121)  3764224 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data
--rw-r--r--   0 runner    (1001) docker     (121)  3129344 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data
--rw-r--r--   0 runner    (1001) docker     (121)  2822144 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data
--rw-r--r--   0 runner    (1001) docker     (121)  2547712 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data
--rw-r--r--   0 runner    (1001) docker     (121)  3735552 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data
--rw-r--r--   0 runner    (1001) docker     (121)  3551232 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data
--rw-r--r--   0 runner    (1001) docker     (121)   983040 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data
--rw-r--r--   0 runner    (1001) docker     (121)   937984 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data
--rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_design_optimizer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    42435 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_design_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_optimizer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    17564 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_test_suite.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/strategy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/test_suite_result.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/strategy_optimizer/test_suite_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/task_manager.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/task_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.883619 OctoBot-0.4.8/octobot/updater/
--rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/binary_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7590 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/binary_updater.py
--rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/python_updater.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/python_updater.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/updater.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/updater.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/updater_factory.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-04 12:11:04.000000 OctoBot-0.4.8/octobot/updater/updater_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-04 12:11:04.000000 OctoBot-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-04 12:12:18.899619 OctoBot-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-09-04 12:11:04.000000 OctoBot-0.4.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-09-04 12:11:04.000000 OctoBot-0.4.8/start.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.827618 OctoBot-0.4.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.887619 OctoBot-0.4.8/tests/functional_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.887619 OctoBot-0.4.8/tests/functional_tests/backtesting_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/backtesting_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/backtesting_tests/backtesting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.887619 OctoBot-0.4.8/tests/functional_tests/evaluators_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/evaluators_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20057 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/evaluators_tests/abstract_TA_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.887619 OctoBot-0.4.8/tests/functional_tests/launch_test/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/launch_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/launch_test/launch_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.887619 OctoBot-0.4.8/tests/functional_tests/strategy_evaluators_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/strategy_evaluators_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.891619 OctoBot-0.4.8/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/bot_management.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     8350 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/data_bank.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/memory_check_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/test_utils/order_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.891619 OctoBot-0.4.8/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.891619 OctoBot-0.4.8/tests/unit_tests/community/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.895619 OctoBot-0.4.8/tests/unit_tests/community/errors_upload/
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/errors_upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_error_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    10462 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_errors_uploader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_initializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    25427 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/test_community_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/test_community_mqtt_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)    12917 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/community/test_community_ws_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.895619 OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/test_configuration_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.895619 OctoBot-0.4.8/tests/unit_tests/trading_modes_tests/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/trading_modes_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9927 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 12:12:18.895619 OctoBot-0.4.8/tests/unit_tests/updater/
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-04 12:11:04.000000 OctoBot-0.4.8/tests/unit_tests/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    51224 2022-09-07 23:11:33.000000 OctoBot-0.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-09-07 23:11:33.000000 OctoBot-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      133 2022-09-07 23:11:33.000000 OctoBot-0.4.9/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.665871 OctoBot-0.4.9/OctoBot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6965 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-07 23:12:40.000000 OctoBot-0.4.9/OctoBot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8885 2022-09-07 23:12:40.733871 OctoBot-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8236 2022-09-07 23:11:33.000000 OctoBot-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.669871 OctoBot-0.4.9/octobot/
+-rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.669871 OctoBot-0.4.9/octobot/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4434 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/api/backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5259 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/api/strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/api/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.669871 OctoBot-0.4.9/octobot/backtesting/
+-rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/abstract_backtesting_test.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    12060 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/abstract_backtesting_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2449 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/independent_backtesting.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    22103 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/independent_backtesting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/octobot_backtesting.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    13942 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/backtesting/octobot_backtesting.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.673871 OctoBot-0.4.9/octobot/channels/
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/channels/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/channels/octobot_channel.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4931 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/channels/octobot_channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19570 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7573 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.673871 OctoBot-0.4.9/octobot/community/
+-rw-r--r--   0 runner    (1001) docker     (121)     3201 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22985 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7359 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_donation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14861 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_supports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_tentacles_package.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3040 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/community_user_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.673871 OctoBot-0.4.9/octobot/community/errors_upload/
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/errors_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/errors_upload/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/errors_upload/errors_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/errors_upload/initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.673871 OctoBot-0.4.9/octobot/community/feeds/
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1705 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/feeds/abstract_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13187 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/feeds/community_mqtt_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11239 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/feeds/community_ws_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/feeds/feed_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/graphql_requests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4124 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/community/identifiers_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.677871 OctoBot-0.4.9/octobot/config/
+-rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/config/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/config/default_config.json
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/config/logging_config.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/config/profile_schema.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/configuration_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10995 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8009 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/initializer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15341 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2576 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7280 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3053 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_backtesting_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_backtesting_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_channel_consumer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     6014 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/octobot_channel_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.677871 OctoBot-0.4.9/octobot/producers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/evaluator_producer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/evaluator_producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/exchange_producer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3389 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/exchange_producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/interface_producer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     9203 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/interface_producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/service_feed_producer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/producers/service_feed_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.681871 OctoBot-0.4.9/octobot/strategy_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.725871 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/
+-rw-r--r--   0 runner    (1001) docker     (121)   950272 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data
+-rw-r--r--   0 runner    (1001) docker     (121)   937984 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data
+-rw-r--r--   0 runner    (1001) docker     (121)   942080 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data
+-rw-r--r--   0 runner    (1001) docker     (121)   958464 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data
+-rw-r--r--   0 runner    (1001) docker     (121)   876544 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data
+-rw-r--r--   0 runner    (1001) docker     (121)   978944 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data
+-rw-r--r--   0 runner    (1001) docker     (121)   946176 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data
+-rw-r--r--   0 runner    (1001) docker     (121)   913408 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data
+-rw-r--r--   0 runner    (1001) docker     (121)  3764224 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data
+-rw-r--r--   0 runner    (1001) docker     (121)  3129344 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data
+-rw-r--r--   0 runner    (1001) docker     (121)  2822144 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data
+-rw-r--r--   0 runner    (1001) docker     (121)  2547712 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data
+-rw-r--r--   0 runner    (1001) docker     (121)  3735552 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data
+-rw-r--r--   0 runner    (1001) docker     (121)  3551232 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data
+-rw-r--r--   0 runner    (1001) docker     (121)   983040 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data
+-rw-r--r--   0 runner    (1001) docker     (121)   937984 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data
+-rw-r--r--   0 runner    (1001) docker     (121)      782 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_design_optimizer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    42435 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_design_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_optimizer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    17564 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_test_suite.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     6502 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/strategy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1441 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/test_suite_result.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3907 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/strategy_optimizer/test_suite_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/task_manager.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5589 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/task_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/octobot/updater/
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1288 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/binary_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7590 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/binary_updater.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1360 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/python_updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/python_updater.py
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/updater.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/updater.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/updater_factory.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-09-07 23:11:33.000000 OctoBot-0.4.9/octobot/updater/updater_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)      382 2022-09-07 23:11:33.000000 OctoBot-0.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-07 23:12:40.733871 OctoBot-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     4234 2022-09-07 23:11:33.000000 OctoBot-0.4.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      864 2022-09-07 23:11:33.000000 OctoBot-0.4.9/start.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.661871 OctoBot-0.4.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/functional_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/functional_tests/backtesting_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/backtesting_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/backtesting_tests/backtesting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/functional_tests/evaluators_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/evaluators_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20057 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/evaluators_tests/abstract_TA_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/functional_tests/launch_test/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/launch_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/launch_test/launch_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/functional_tests/strategy_evaluators_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/strategy_evaluators_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.729871 OctoBot-0.4.9/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/bot_management.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8350 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/data_bank.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/memory_check_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/test_utils/order_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/community/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/community/errors_upload/
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/errors_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3152 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10462 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_errors_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25427 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      929 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/test_community_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7337 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/test_community_mqtt_feed.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12917 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/community/test_community_ws_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2615 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/test_configuration_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/trading_modes_tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/trading_modes_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9927 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-07 23:12:40.733871 OctoBot-0.4.9/tests/unit_tests/updater/
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-09-07 23:11:33.000000 OctoBot-0.4.9/tests/unit_tests/updater/test_updater.py
```

### Comparing `OctoBot-0.4.8/CHANGELOG.md` & `OctoBot-0.4.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 *It is strongly advised to perform an update of your tentacles after updating OctoBot. (start.py tentacles --install --all)*
 
+## [0.4.9] - 2022-09-07
+### Updated
+- Beta tentacles
+### Fixed
+- Profile export
+
 ## [0.4.8] - 2022-09-04
 ### Fixed
 - Device creation
 
 ## [0.4.7] - 2022-09-03
 ### Updated
 - [Astrolab] Improvements and fixes
```

### Comparing `OctoBot-0.4.8/LICENSE` & `OctoBot-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/OctoBot.egg-info/PKG-INFO` & `OctoBot-0.4.9/OctoBot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cryptocurrencies alert / trading bot
 Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# OctoBot [0.4.8](https://octobot.click/gh-changelog)
+# OctoBot [0.4.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg)](https://octobot.click/gh-pypi)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-Software/OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)](https://octobot.click/gh-dockerhub)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot/badge.svg?branch=dev)](https://coveralls.io/github/Drakkar-Software/OctoBot?branch=dev)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot)
 [![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: OctoBot Version: 0.4.8 Summary: Cryptocurrencies
+Metadata-Version: 2.1 Name: OctoBot Version: 0.4.9 Summary: Cryptocurrencies
 alert / trading bot Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software Author-email: drakkar-software@protonmail.com License:
 GPL-3.0 Classifier: Development Status :: 4 - Beta Classifier: Operating System
 :: OS Independent Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Cython Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE # OctoBot [0.4.8](https://octobot.click/gh-
+markdown License-File: LICENSE # OctoBot [0.4.9](https://octobot.click/gh-
 changelog) [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg)](https://
 octobot.click/gh-pypi) [![Codacy Badge](https://api.codacy.com/project/badge/
 Grade/e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-
 Software/OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-
 Software/OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://
 pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot) [!
 [Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)]
```

### Comparing `OctoBot-0.4.8/OctoBot.egg-info/SOURCES.txt` & `OctoBot-0.4.9/OctoBot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/PKG-INFO` & `OctoBot-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OctoBot
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cryptocurrencies alert / trading bot
 Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software
 Author-email: drakkar-software@protonmail.com
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Cython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# OctoBot [0.4.8](https://octobot.click/gh-changelog)
+# OctoBot [0.4.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg)](https://octobot.click/gh-pypi)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-Software/OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)](https://octobot.click/gh-dockerhub)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot/badge.svg?branch=dev)](https://coveralls.io/github/Drakkar-Software/OctoBot?branch=dev)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot)
 [![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: OctoBot Version: 0.4.8 Summary: Cryptocurrencies
+Metadata-Version: 2.1 Name: OctoBot Version: 0.4.9 Summary: Cryptocurrencies
 alert / trading bot Home-page: https://github.com/Drakkar-Software/OctoBot
 Author: Drakkar-Software Author-email: drakkar-software@protonmail.com License:
 GPL-3.0 Classifier: Development Status :: 4 - Beta Classifier: Operating System
 :: OS Independent Classifier: Operating System :: MacOS :: MacOS X Classifier:
 Operating System :: Microsoft :: Windows Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Cython Requires-Python: >=3.8 Description-Content-Type: text/
-markdown License-File: LICENSE # OctoBot [0.4.8](https://octobot.click/gh-
+markdown License-File: LICENSE # OctoBot [0.4.9](https://octobot.click/gh-
 changelog) [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg)](https://
 octobot.click/gh-pypi) [![Codacy Badge](https://api.codacy.com/project/badge/
 Grade/e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-
 Software/OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-
 Software/OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://
 pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot) [!
 [Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)]
```

### Comparing `OctoBot-0.4.8/README.md` & `OctoBot-0.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# OctoBot [0.4.8](https://octobot.click/gh-changelog)
+# OctoBot [0.4.9](https://octobot.click/gh-changelog)
 [![PyPI](https://img.shields.io/pypi/v/OctoBot.svg)](https://octobot.click/gh-pypi)
 [![Codacy Badge](https://api.codacy.com/project/badge/Grade/e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-Software/OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://pepy.tech/badge/octobot/month)](https://pepy.tech/project/octobot)
 [![Dockerhub](https://img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)](https://octobot.click/gh-dockerhub)
 [![Coverage Status](https://coveralls.io/repos/github/Drakkar-Software/OctoBot/badge.svg?branch=dev)](https://coveralls.io/github/Drakkar-Software/OctoBot?branch=dev)
 [![OctoBot-CI](https://github.com/Drakkar-Software/OctoBot/workflows/OctoBot-CI/badge.svg)](https://github.com/Drakkar-Software/OctoBot/actions)
 [![Build Status](https://cloud.drone.io/api/badges/Drakkar-Software/OctoBot/status.svg)](https://cloud.drone.io/Drakkar-Software/OctoBot)
 [![UptimeRobot](https://img.shields.io/uptimerobot/ratio/30/m786447893-903b482e5158c8b6483760e8)](https://octobot.click/gh-status)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# OctoBot [0.4.8](https://octobot.click/gh-changelog) [![PyPI](https://
+# OctoBot [0.4.9](https://octobot.click/gh-changelog) [![PyPI](https://
 img.shields.io/pypi/v/OctoBot.svg)](https://octobot.click/gh-pypi) [![Codacy
 Badge](https://api.codacy.com/project/badge/Grade/
 e07fb190156d4efb8e7d07aaa5eff2e1)](https://app.codacy.com/gh/Drakkar-Software/
 OctoBot?utm_source=github.com&utm_medium=referral&utm_content=Drakkar-Software/
 OctoBot&utm_campaign=Badge_Grade_Dashboard)[![Downloads](https://pepy.tech/
 badge/octobot/month)](https://pepy.tech/project/octobot) [![Dockerhub](https://
 img.shields.io/docker/pulls/drakkarsoftware/octobot.svg)](https://
```

### Comparing `OctoBot-0.4.8/octobot/__init__.pxd` & `OctoBot-0.4.9/octobot/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/__init__.py` & `OctoBot-0.4.9/octobot/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/api/__init__.py` & `OctoBot-0.4.9/octobot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/api/backtesting.py` & `OctoBot-0.4.9/octobot/api/backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/api/strategy_optimizer.py` & `OctoBot-0.4.9/octobot/api/strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/api/updater.py` & `OctoBot-0.4.9/octobot/api/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/__init__.pxd` & `OctoBot-0.4.9/octobot/backtesting/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/__init__.py` & `OctoBot-0.4.9/octobot/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/abstract_backtesting_test.pxd` & `OctoBot-0.4.9/octobot/backtesting/abstract_backtesting_test.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/abstract_backtesting_test.py` & `OctoBot-0.4.9/octobot/backtesting/abstract_backtesting_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/independent_backtesting.pxd` & `OctoBot-0.4.9/octobot/backtesting/independent_backtesting.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/independent_backtesting.py` & `OctoBot-0.4.9/octobot/backtesting/independent_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/octobot_backtesting.pxd` & `OctoBot-0.4.9/octobot/backtesting/octobot_backtesting.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/backtesting/octobot_backtesting.py` & `OctoBot-0.4.9/octobot/backtesting/octobot_backtesting.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/channels/__init__.pxd` & `OctoBot-0.4.9/octobot/channels/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/channels/__init__.py` & `OctoBot-0.4.9/octobot/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/channels/octobot_channel.pxd` & `OctoBot-0.4.9/octobot/channels/octobot_channel.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/channels/octobot_channel.py` & `OctoBot-0.4.9/octobot/channels/octobot_channel.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/cli.py` & `OctoBot-0.4.9/octobot/cli.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/commands.py` & `OctoBot-0.4.9/octobot/commands.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/__init__.py` & `OctoBot-0.4.9/octobot/community/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/authentication.py` & `OctoBot-0.4.9/octobot/community/authentication.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_analysis.py` & `OctoBot-0.4.9/octobot/community/community_analysis.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_donation.py` & `OctoBot-0.4.9/octobot/community/community_donation.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_fields.py` & `OctoBot-0.4.9/octobot/community/community_fields.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_manager.py` & `OctoBot-0.4.9/octobot/community/community_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_supports.py` & `OctoBot-0.4.9/octobot/community/community_supports.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_tentacles_package.py` & `OctoBot-0.4.9/octobot/community/community_tentacles_package.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/community_user_account.py` & `OctoBot-0.4.9/octobot/community/community_user_account.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/errors.py` & `OctoBot-0.4.9/octobot/community/errors.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/errors_upload/__init__.py` & `OctoBot-0.4.9/octobot/community/errors_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/errors_upload/error_model.py` & `OctoBot-0.4.9/octobot/community/errors_upload/error_model.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/errors_upload/errors_uploader.py` & `OctoBot-0.4.9/octobot/community/errors_upload/errors_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/errors_upload/initializer.py` & `OctoBot-0.4.9/octobot/community/errors_upload/initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/feeds/__init__.py` & `OctoBot-0.4.9/octobot/community/feeds/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/feeds/abstract_feed.py` & `OctoBot-0.4.9/octobot/community/feeds/abstract_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/feeds/community_mqtt_feed.py` & `OctoBot-0.4.9/octobot/community/feeds/community_mqtt_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/feeds/community_ws_feed.py` & `OctoBot-0.4.9/octobot/community/feeds/community_ws_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/feeds/feed_factory.py` & `OctoBot-0.4.9/octobot/community/feeds/feed_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/graphql_requests.py` & `OctoBot-0.4.9/octobot/community/graphql_requests.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/community/identifiers_provider.py` & `OctoBot-0.4.9/octobot/community/identifiers_provider.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/config/config_schema.json` & `OctoBot-0.4.9/octobot/config/config_schema.json`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/config/logging_config.ini` & `OctoBot-0.4.9/octobot/config/logging_config.ini`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/config/profile_schema.json` & `OctoBot-0.4.9/octobot/config/profile_schema.json`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/configuration_manager.pxd` & `OctoBot-0.4.9/octobot/configuration_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/configuration_manager.py` & `OctoBot-0.4.9/octobot/configuration_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import shutil
 import json
 
 import octobot.constants as constants
 import octobot_commons.configuration as configuration
 import octobot_commons.constants as common_constants
 import octobot_commons.logging as logging
+import octobot_commons.errors as common_errors
 import octobot_tentacles_manager.constants as tentacles_manager_constants
 
 import octobot_trading.api as trading_api
 
 LOGGER_NAME = "Configuration"
 
 
@@ -140,21 +141,27 @@
         default_config = json.loads(default_config_file.read())
     default_profile_id = default_config.get(common_constants.CONFIG_PROFILE)
     config.select_profile(default_profile_id)
     config.save()
 
 
 def get_default_tentacles_url(version=None):
+    beta_tentacle_bundle = os.getenv(constants.ENV_BETA_TENTACLES_PACKAGE_NAME, constants.BETA_TENTACLE_PACKAGE_NAME)
+    # use beta tentacles repository for beta tentacles
+    tentacles_repository = \
+        os.getenv(constants.ENV_BETA_TENTACLES_REPOSITORY, constants.BETA_TENTACLES_REPOSITORY) \
+        if version == beta_tentacle_bundle else \
+        os.getenv(constants.ENV_TENTACLES_REPOSITORY, constants.TENTACLES_REPOSITORY)
     if version is None:
         version = constants.TENTACLES_REQUIRED_VERSION \
             if constants.TENTACLES_REQUIRED_VERSION else constants.LONG_VERSION
     return os.getenv(
         constants.ENV_TENTACLES_URL,
         f"{constants.OCTOBOT_ONLINE}/"
-        f"{os.getenv(constants.ENV_TENTACLES_REPOSITORY, constants.TENTACLES_REPOSITORY)}/"
+        f"{tentacles_repository}/"
         f"{os.getenv(constants.ENV_TENTACLES_PACKAGES_SOURCE, constants.OFFICIALS)}/"
         f"{os.getenv(constants.ENV_TENTACLES_PACKAGES_TYPE, constants.TENTACLE_PACKAGES)}/"
         f"{os.getenv(constants.ENV_TENTACLE_CATEGORY, constants.TENTACLE_CATEGORY)}/"
         f"{os.getenv(constants.ENV_TENTACLE_PACKAGE_NAME, constants.TENTACLE_PACKAGE_NAME)}/"
         f"{version}/"
         f"{tentacles_manager_constants.ANY_PLATFORM_FILE_NAME}.{tentacles_manager_constants.TENTACLES_PACKAGE_FORMAT}"
     )
```

### Comparing `OctoBot-0.4.8/octobot/constants.py` & `OctoBot-0.4.9/octobot/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,32 +16,34 @@
 import os
 import pathlib
 import octobot_commons.os_util as os_util
 import octobot.enums
 
 PROJECT_NAME = "OctoBot"
 AUTHOR = "DrakkarSoftware"
-SHORT_VERSION = "0.4.8"  # major.minor.revision
+SHORT_VERSION = "0.4.9"  # major.minor.revision
 PATCH_VERSION = ""  # patch : pX
 VERSION_DEV_PHASE = ""  # alpha : a / beta : b / release candidate : rc
 VERSION_PHASE = ""  # XX
 VERSION = f"{SHORT_VERSION}{VERSION_DEV_PHASE}{VERSION_PHASE}"
 LONG_VERSION = f"{SHORT_VERSION}{PATCH_VERSION}{VERSION_DEV_PHASE}{VERSION_PHASE}"
 
 # OctoBot urls
 OCTOBOT_WEBSITE_URL = os.getenv("OCTOBOT_ONLINE_URL", "https://www.octobot.online")
 OCTOBOT_DOCS_URL = os.getenv("DOCS_OCTOBOT_ONLINE_URL", "https://www.octobot.info")
 EXCHANGES_DOCS_URL = os.getenv("DOCS_OCTOBOT_ONLINE_URL", "https://exchanges.octobot.info/")
 DEVELOPER_DOCS_URL = os.getenv("DOCS_OCTOBOT_ONLINE_URL", "https://developer.octobot.info/")
 OCTOBOT_ONLINE = os.getenv("TENTACLES_OCTOBOT_ONLINE_URL", "https://static.octobot.online")
 OCTOBOT_FEEDBACK = os.getenv("FEEDBACK_OCTOBOT_ONLINE_URL", "https://feedback.octobot.online/")
 TENTACLES_REPOSITORY = "tentacles"
+BETA_TENTACLES_REPOSITORY = "dev-tentacles"
 OFFICIALS = "officials"
 TENTACLE_CATEGORY = "full"
 TENTACLE_PACKAGE_NAME = "base"
+BETA_TENTACLE_PACKAGE_NAME = "beta"
 TENTACLE_PACKAGES = "packages"
 COMPILED_TENTACLE_CATEGORY = "extra"
 
 OCTOBOT_DONATION_URL = "https://forms.gle/Bagagc7dyjJGDT1t9"
 OCTOBOT_FEEDBACK_FORM_URL = "https://goo.gl/forms/vspraniXPY7rvtKN2"
 OCTOBOT_BETA_PROGRAM_FORM_URL = "https://forms.gle/igqn1TjQ8XVA1dXBA"
 
@@ -88,16 +90,18 @@
 
 OCTOBOT_BINARY_PROJECT_NAME = "OctoBot-Binary"
 
 # tentacles
 ENV_TENTACLES_URL = "TENTACLES_URL"
 ENV_COMPILED_TENTACLES_URL = "COMPILED_TENTACLES_URL"
 ENV_TENTACLES_REPOSITORY = "TENTACLES_REPOSITORY"
+ENV_BETA_TENTACLES_REPOSITORY = "BETA_TENTACLES_REPOSITORY"
 ENV_TENTACLES_URL_TAG = "TENTACLES_URL_TAG"
 ENV_TENTACLE_PACKAGE_NAME = "TENTACLE_PACKAGE_NAME"
+ENV_BETA_TENTACLES_PACKAGE_NAME = "BETA_TENTACLES_PACKAGE_NAME"
 ENV_TENTACLES_PACKAGES_TYPE = "TENTACLES_PACKAGES_TYPE"
 ENV_TENTACLES_PACKAGES_SOURCE = "TENTACLES_PACKAGES_SOURCE"
 ENV_COMPILED_TENTACLES_CATEGORY = "COMPILED_TENTACLES_CATEGORY"
 ENV_COMPILED_TENTACLES_PACKAGES_TYPE = "COMPILED_TENTACLES_PACKAGES_TYPE"
 ENV_TENTACLE_CATEGORY = "TENTACLE_CATEGORY"
 ENV_COMPILED_TENTACLES_SUBCATEGORY = "COMPILED_TENTACLES_SUBCATEGORY"
 TENTACLES_REQUIRED_VERSION = f"{os.getenv(ENV_TENTACLES_URL_TAG, LONG_VERSION)}"
```

### Comparing `OctoBot-0.4.8/octobot/disclaimer.py` & `OctoBot-0.4.9/octobot/disclaimer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/enums.py` & `OctoBot-0.4.9/octobot/enums.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/initializer.pxd` & `OctoBot-0.4.9/octobot/initializer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/initializer.py` & `OctoBot-0.4.9/octobot/initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/logger.py` & `OctoBot-0.4.9/octobot/logger.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot.pxd` & `OctoBot-0.4.9/octobot/octobot.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot.py` & `OctoBot-0.4.9/octobot/octobot.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_api.pxd` & `OctoBot-0.4.9/octobot/octobot_api.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_api.py` & `OctoBot-0.4.9/octobot/octobot_api.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_backtesting_factory.pxd` & `OctoBot-0.4.9/octobot/octobot_backtesting_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_backtesting_factory.py` & `OctoBot-0.4.9/octobot/octobot_backtesting_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_channel_consumer.pxd` & `OctoBot-0.4.9/octobot/octobot_channel_consumer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/octobot_channel_consumer.py` & `OctoBot-0.4.9/octobot/octobot_channel_consumer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/__init__.pxd` & `OctoBot-0.4.9/octobot/producers/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/__init__.py` & `OctoBot-0.4.9/octobot/producers/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/evaluator_producer.pxd` & `OctoBot-0.4.9/octobot/producers/evaluator_producer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/evaluator_producer.py` & `OctoBot-0.4.9/octobot/producers/evaluator_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/exchange_producer.pxd` & `OctoBot-0.4.9/octobot/producers/exchange_producer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/exchange_producer.py` & `OctoBot-0.4.9/octobot/producers/exchange_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/interface_producer.pxd` & `OctoBot-0.4.9/octobot/producers/interface_producer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/interface_producer.py` & `OctoBot-0.4.9/octobot/producers/interface_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/service_feed_producer.pxd` & `OctoBot-0.4.9/octobot/producers/service_feed_producer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/producers/service_feed_producer.py` & `OctoBot-0.4.9/octobot/producers/service_feed_producer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/__init__.pxd` & `OctoBot-0.4.9/octobot/strategy_optimizer/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/__init__.py` & `OctoBot-0.4.9/octobot/strategy_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774950.9324272.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774962.1269426.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774974.669779.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774982.726014.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774988.7215023.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581774995.2311237.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775018.2658834.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775026.9255266.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775117.1713624.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775133.1533682.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775139.0332782.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775144.480404.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775149.6372743.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581775154.2598503.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776404.9679003.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data` & `OctoBot-0.4.9/octobot/strategy_optimizer/optimizer_data_files/AbstractExchangeHistoryCollector_1581776676.5721796.data`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_design_optimizer.pxd` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_design_optimizer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_design_optimizer.py` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_design_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_optimizer.pxd` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_optimizer.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_optimizer.py` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_test_suite.pxd` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_test_suite.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/strategy_test_suite.py` & `OctoBot-0.4.9/octobot/strategy_optimizer/strategy_test_suite.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/test_suite_result.pxd` & `OctoBot-0.4.9/octobot/strategy_optimizer/test_suite_result.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/strategy_optimizer/test_suite_result.py` & `OctoBot-0.4.9/octobot/strategy_optimizer/test_suite_result.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/task_manager.pxd` & `OctoBot-0.4.9/octobot/task_manager.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/task_manager.py` & `OctoBot-0.4.9/octobot/task_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/__init__.pxd` & `OctoBot-0.4.9/octobot/updater/__init__.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/__init__.py` & `OctoBot-0.4.9/octobot/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/binary_updater.pxd` & `OctoBot-0.4.9/octobot/updater/binary_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/binary_updater.py` & `OctoBot-0.4.9/octobot/updater/binary_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/python_updater.pxd` & `OctoBot-0.4.9/octobot/updater/python_updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/python_updater.py` & `OctoBot-0.4.9/octobot/updater/python_updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/updater.pxd` & `OctoBot-0.4.9/octobot/updater/updater.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/updater.py` & `OctoBot-0.4.9/octobot/updater/updater.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/updater_factory.pxd` & `OctoBot-0.4.9/octobot/updater/updater_factory.pxd`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/octobot/updater/updater_factory.py` & `OctoBot-0.4.9/octobot/updater/updater_factory.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/setup.py` & `OctoBot-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/start.py` & `OctoBot-0.4.9/start.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/__init__.py` & `OctoBot-0.4.9/tests/functional_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/backtesting_tests/__init__.py` & `OctoBot-0.4.9/tests/functional_tests/backtesting_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/backtesting_tests/backtesting_test.py` & `OctoBot-0.4.9/tests/functional_tests/backtesting_tests/backtesting_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/evaluators_tests/__init__.py` & `OctoBot-0.4.9/tests/functional_tests/evaluators_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/evaluators_tests/abstract_TA_test.py` & `OctoBot-0.4.9/tests/functional_tests/evaluators_tests/abstract_TA_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/launch_test/__init__.py` & `OctoBot-0.4.9/tests/functional_tests/launch_test/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/launch_test/launch_test.py` & `OctoBot-0.4.9/tests/functional_tests/launch_test/launch_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/strategy_evaluators_tests/__init__.py` & `OctoBot-0.4.9/tests/functional_tests/strategy_evaluators_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py` & `OctoBot-0.4.9/tests/functional_tests/strategy_evaluators_tests/abstract_strategy_test.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/__init__.py` & `OctoBot-0.4.9/tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/bot_management.py` & `OctoBot-0.4.9/tests/test_utils/bot_management.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/config.py` & `OctoBot-0.4.9/tests/test_utils/config.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/data_bank.py` & `OctoBot-0.4.9/tests/test_utils/data_bank.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/logging.py` & `OctoBot-0.4.9/tests/test_utils/logging.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/memory_check_util.py` & `OctoBot-0.4.9/tests/test_utils/memory_check_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/test_utils/order_util.py` & `OctoBot-0.4.9/tests/test_utils/order_util.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/__init__.py` & `OctoBot-0.4.9/tests/unit_tests/community/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/errors_upload/__init__.py` & `OctoBot-0.4.9/tests/unit_tests/community/errors_upload/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_error_model.py` & `OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_error_model.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_errors_uploader.py` & `OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_errors_uploader.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/errors_upload/test_initializer.py` & `OctoBot-0.4.9/tests/unit_tests/community/errors_upload/test_initializer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/test_authentication.py` & `OctoBot-0.4.9/tests/unit_tests/community/test_authentication.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/test_community_data.py` & `OctoBot-0.4.9/tests/unit_tests/community/test_community_data.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/test_community_mqtt_feed.py` & `OctoBot-0.4.9/tests/unit_tests/community/test_community_mqtt_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/community/test_community_ws_feed.py` & `OctoBot-0.4.9/tests/unit_tests/community/test_community_ws_feed.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/__init__.py` & `OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py` & `OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/test_strategy_optimizer.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py` & `OctoBot-0.4.9/tests/unit_tests/strategy_optimizer/test_strategy_test_suite.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/test_configuration_manager.py` & `OctoBot-0.4.9/tests/unit_tests/test_configuration_manager.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/trading_modes_tests/__init__.py` & `OctoBot-0.4.9/tests/unit_tests/trading_modes_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py` & `OctoBot-0.4.9/tests/unit_tests/trading_modes_tests/trading_mode_test_toolkit.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/updater/__init__.py` & `OctoBot-0.4.9/tests/unit_tests/updater/__init__.py`

 * *Files identical despite different names*

### Comparing `OctoBot-0.4.8/tests/unit_tests/updater/test_updater.py` & `OctoBot-0.4.9/tests/unit_tests/updater/test_updater.py`

 * *Files identical despite different names*

