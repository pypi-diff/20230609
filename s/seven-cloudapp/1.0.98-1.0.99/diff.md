# Comparing `tmp/seven_cloudapp-1.0.98.tar.gz` & `tmp/seven_cloudapp-1.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seven_cloudapp-1.0.98.tar", last modified: Thu Dec 17 03:44:00 2020, max compression
+gzip compressed data, was "dist\seven_cloudapp-1.0.99.tar", last modified: Thu Dec 17 07:22:38 2020, max compression
```

## Comparing `seven_cloudapp-1.0.98.tar` & `seven_cloudapp-1.0.99.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.775818 seven_cloudapp-1.0.98/
--rw-rw-rw-   0        0        0     3839 2020-12-17 03:44:00.774820 seven_cloudapp-1.0.98/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2020-12-17 03:43:42.000000 seven_cloudapp-1.0.98/README.md
--rw-rw-rw-   0        0        0       42 2020-12-17 03:44:00.776815 seven_cloudapp-1.0.98/setup.cfg
--rw-rw-rw-   0        0        0     1292 2020-12-17 03:42:25.000000 seven_cloudapp-1.0.98/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.539939 seven_cloudapp-1.0.98/seven_cloudapp/
--rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.555896 seven_cloudapp-1.0.98/seven_cloudapp/handlers/
--rw-rw-rw-   0        0        0      186 2020-05-26 07:27:31.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.574845 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/
--rw-rw-rw-   0        0        0      260 2020-11-20 08:18:12.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/__init__.py
--rw-rw-rw-   0        0        0     1479 2020-12-16 09:26:24.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/act.py
--rw-rw-rw-   0        0        0   411235 2020-11-03 10:29:20.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/address.py
--rw-rw-rw-   0        0        0     1279 2020-11-20 08:22:54.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/app.py
--rw-rw-rw-   0        0        0     4024 2020-12-16 09:29:25.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/goods.py
--rw-rw-rw-   0        0        0      552 2020-11-10 08:02:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/lottery.py
--rw-rw-rw-   0        0        0     1421 2020-11-24 09:25:14.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/machine.py
--rw-rw-rw-   0        0        0     9391 2020-12-09 10:28:29.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/prize.py
--rw-rw-rw-   0        0        0     7943 2020-11-05 09:31:06.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/theme.py
--rw-rw-rw-   0        0        0     7369 2020-12-16 06:29:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/user.py
--rw-rw-rw-   0        0        0      546 2020-12-16 02:49:49.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/core.py
--rw-rw-rw-   0        0        0     1678 2020-09-07 09:02:32.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/monitor.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.597785 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/
--rw-rw-rw-   0        0        0      314 2020-08-12 10:23:42.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/__init__.py
--rw-rw-rw-   0        0        0    17128 2020-12-16 03:14:58.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/act_s.py
--rw-rw-rw-   0        0        0    12288 2020-12-10 09:01:19.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/app_s.py
--rw-rw-rw-   0        0        0     6634 2020-12-16 03:16:15.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/base_s.py
--rw-rw-rw-   0        0        0     7385 2020-12-16 05:59:06.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/goods_s.py
--rw-rw-rw-   0        0        0     6229 2020-12-16 03:50:26.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/machine_s.py
--rw-rw-rw-   0        0        0    19841 2020-12-17 03:21:04.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/order_s.py
--rw-rw-rw-   0        0        0    10870 2020-12-16 01:42:56.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/price_s.py
--rw-rw-rw-   0        0        0    14654 2020-12-16 07:12:02.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/prize_s.py
--rw-rw-rw-   0        0        0    12404 2020-12-10 03:21:07.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/report_s.py
--rw-rw-rw-   0        0        0     1853 2020-11-04 08:20:01.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/sms_s.py
--rw-rw-rw-   0        0        0     3481 2020-11-04 08:46:59.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/theme_s.py
--rw-rw-rw-   0        0        0    15180 2020-12-16 03:22:14.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/throw_s.py
--rw-rw-rw-   0        0        0    15957 2020-12-17 03:41:13.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/user_s.py
--rw-rw-rw-   0        0        0    15160 2020-12-16 06:31:36.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/seven_base.py
--rw-rw-rw-   0        0        0    38605 2020-12-16 05:53:16.000000 seven_cloudapp-1.0.98/seven_cloudapp/handlers/top_base.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.599779 seven_cloudapp-1.0.98/seven_cloudapp/libs/
--rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.605764 seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/
--rw-rw-rw-   0        0        0      196 2020-05-26 07:27:31.000000 seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/__init__.py
--rw-rw-rw-   0        0        0     2812 2020-12-07 08:26:14.000000 seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/oss2help.py
--rw-rw-rw-   0        0        0     5492 2020-11-24 01:55:28.000000 seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/seven.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.629699 seven_cloudapp-1.0.98/seven_cloudapp/models/
--rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/__init__.py
--rw-rw-rw-   0        0        0    11184 2020-12-11 07:06:48.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/behavior_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.632692 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/
--rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/__init__.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.640669 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/
--rw-rw-rw-   0        0        0       62 2020-12-16 10:16:02.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/__init__.py
--rw-rw-rw-   0        0        0     2679 2020-12-11 07:30:19.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_info_model.py
--rw-rw-rw-   0        0        0     3508 2020-12-16 10:18:22.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_prize_model.py
--rw-rw-rw-   0        0        0     2302 2020-12-16 10:14:23.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_type_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.644659 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/app/
--rw-rw-rw-   0        0        0       26 2020-11-18 02:15:07.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/app/__init__.py
--rw-rw-rw-   0        0        0     2471 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/app/app_info_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.647650 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/base/
--rw-rw-rw-   0        0        0       28 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/base/__init__.py
--rw-rw-rw-   0        0        0     2605 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/base/base_info_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.653634 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/
--rw-rw-rw-   0        0        0       75 2020-11-18 02:14:40.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/__init__.py
--rw-rw-rw-   0        0        0     1199 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_log_model.py
--rw-rw-rw-   0        0        0     1901 2020-12-16 08:51:15.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_orm_model.py
--rw-rw-rw-   0        0        0     1402 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_report_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.655629 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/browse/
--rw-rw-rw-   0        0        0       29 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/browse/__init__.py
--rw-rw-rw-   0        0        0     1281 2020-11-19 06:02:05.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/browse/browse_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.658622 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/coin/
--rw-rw-rw-   0        0        0       28 2020-11-18 02:14:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/coin/__init__.py
--rw-rw-rw-   0        0        0     2107 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/coin/coin_order_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.662611 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/collect/
--rw-rw-rw-   0        0        0       30 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/collect/__init__.py
--rw-rw-rw-   0        0        0     1287 2020-11-19 05:47:07.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/collect/collect_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.665603 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/consume/
--rw-rw-rw-   0        0        0       35 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/consume/__init__.py
--rw-rw-rw-   0        0        0     1245 2020-11-19 09:15:28.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/consume/consume_gear_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.669592 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/
--rw-rw-rw-   0        0        0       50 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/__init__.py
--rw-rw-rw-   0        0        0     1369 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/course_info_model.py
--rw-rw-rw-   0        0        0     1364 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/course_type_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.672584 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/friend/
--rw-rw-rw-   0        0        0       30 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/friend/__init__.py
--rw-rw-rw-   0        0        0     1536 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/friend/friend_link_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.677571 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/
--rw-rw-rw-   0        0        0       45 2020-11-18 02:14:14.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/__init__.py
--rw-rw-rw-   0        0        0     1482 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/gear_log_model.py
--rw-rw-rw-   0        0        0     1335 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/gear_value_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.680564 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/invite/
--rw-rw-rw-   0        0        0       29 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/invite/__init__.py
--rw-rw-rw-   0        0        0     1370 2020-12-01 03:04:14.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/invite/invite_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.683555 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/login/
--rw-rw-rw-   0        0        0       27 2020-11-18 02:13:56.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/login/__init__.py
--rw-rw-rw-   0        0        0     1357 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/login/login_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.687544 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/
--rw-rw-rw-   0        0        0       56 2020-11-19 08:40:12.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/__init__.py
--rw-rw-rw-   0        0        0     1192 2020-11-19 08:40:12.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/lottery_log_model.py
--rw-rw-rw-   0        0        0     2037 2020-12-15 07:02:47.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/lottery_value_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.695523 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/
--rw-rw-rw-   0        0        0       78 2020-11-18 02:13:15.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/__init__.py
--rw-rw-rw-   0        0        0     2055 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_info_model.py
--rw-rw-rw-   0        0        0     1409 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_value_log_model.py
--rw-rw-rw-   0        0        0     1352 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_value_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.699512 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/marketing/
--rw-rw-rw-   0        0        0       36 2020-12-16 10:16:21.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/marketing/__init__.py
--rw-rw-rw-   0        0        0     1490 2020-12-16 10:14:23.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/marketing/marketing_program_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.703502 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/message/
--rw-rw-rw-   0        0        0       31 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/message/__init__.py
--rw-rw-rw-   0        0        0     2367 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/message/message_info_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.708489 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/middler/
--rw-rw-rw-   0        0        0       48 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/middler/__init__.py
--rw-rw-rw-   0        0        0     1482 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/middler/middler_product_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.713475 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/operation/
--rw-rw-rw-   0        0        0       31 2020-11-18 02:12:53.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/operation/__init__.py
--rw-rw-rw-   0        0        0     1891 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/operation/operation_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.716467 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/pay/
--rw-rw-rw-   0        0        0       27 2020-11-18 02:12:38.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/pay/__init__.py
--rw-rw-rw-   0        0        0     1960 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/pay/pay_order_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.720456 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/price/
--rw-rw-rw-   0        0        0       28 2020-11-18 02:12:23.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/price/__init__.py
--rw-rw-rw-   0        0        0     1318 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/price/price_gear_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.735416 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/
--rw-rw-rw-   0        0        0       50 2020-11-18 02:10:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/__init__.py
--rw-rw-rw-   0        0        0     2062 2020-12-11 07:30:19.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/prize_order_model.py
--rw-rw-rw-   0        0        0     2965 2020-12-15 08:39:02.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/prize_roster_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.739406 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/recommend/
--rw-rw-rw-   0        0        0       34 2020-11-25 07:07:41.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/recommend/__init__.py
--rw-rw-rw-   0        0        0     1343 2020-11-25 07:07:41.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/recommend/recommend_goods_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.743395 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/reward/
--rw-rw-rw-   0        0        0       35 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/reward/__init__.py
--rw-rw-rw-   0        0        0     1333 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/reward/reward_order_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.746895 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/signin/
--rw-rw-rw-   0        0        0       29 2020-11-25 07:21:13.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/signin/__init__.py
--rw-rw-rw-   0        0        0     1266 2020-11-25 07:21:13.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/signin/signin_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.749886 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/skin/
--rw-rw-rw-   0        0        0       27 2020-11-18 02:12:03.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/skin/__init__.py
--rw-rw-rw-   0        0        0     1469 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/skin/skin_info_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.753876 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/
--rw-rw-rw-   0        0        0       47 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/__init__.py
--rw-rw-rw-   0        0        0     1397 2020-11-19 06:09:17.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/task_count_model.py
--rw-rw-rw-   0        0        0     1436 2020-11-19 06:09:17.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/task_info_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.760858 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/
--rw-rw-rw-   0        0        0       46 2020-11-18 02:11:52.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/__init__.py
--rw-rw-rw-   0        0        0     1536 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/theme_info_model.py
--rw-rw-rw-   0        0        0     1200 2020-11-12 09:11:26.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/theme_ver_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.763850 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/throw/
--rw-rw-rw-   0        0        0       29 2020-11-18 02:11:35.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/throw/__init__.py
--rw-rw-rw-   0        0        0     1526 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/throw/throw_goods_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.769833 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/
--rw-rw-rw-   0        0        0       75 2020-11-25 09:47:05.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/__init__.py
--rw-rw-rw-   0        0        0     1688 2020-11-26 07:09:35.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_blacklist_model.py
--rw-rw-rw-   0        0        0     2374 2020-12-11 09:09:01.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_info_model.py
--rw-rw-rw-   0        0        0     1405 2020-11-24 11:20:59.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_unbind_log_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.772825 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/version/
--rw-rw-rw-   0        0        0       31 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/version/__init__.py
--rw-rw-rw-   0        0        0     1488 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/version/version_info_model.py
--rw-rw-rw-   0        0        0     2334 2020-12-01 08:22:05.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/enum.py
--rw-rw-rw-   0        0        0     3159 2020-12-16 01:16:26.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/seven_model.py
--rw-rw-rw-   0        0        0     1943 2020-08-12 10:23:42.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/taobao_model.py
--rw-rw-rw-   0        0        0     4048 2020-12-16 06:24:12.000000 seven_cloudapp-1.0.98/seven_cloudapp/models/throw_model.py
-drwxrwxrwx   0        0        0        0 2020-12-17 03:44:00.547917 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/
--rw-rw-rw-   0        0        0     3839 2020-12-17 03:44:00.000000 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6091 2020-12-17 03:44:00.000000 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-17 03:44:00.000000 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-12-17 03:44:00.000000 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2020-12-17 03:44:00.000000 seven_cloudapp-1.0.98/seven_cloudapp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.184299 seven_cloudapp-1.0.99/
+-rw-rw-rw-   0        0        0     3839 2020-12-17 07:22:38.183301 seven_cloudapp-1.0.99/PKG-INFO
+-rw-rw-rw-   0        0        0     2295 2020-12-17 07:21:03.000000 seven_cloudapp-1.0.99/README.md
+-rw-rw-rw-   0        0        0       42 2020-12-17 07:22:38.185296 seven_cloudapp-1.0.99/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2020-12-17 07:20:58.000000 seven_cloudapp-1.0.99/setup.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:37.939952 seven_cloudapp-1.0.99/seven_cloudapp/
+-rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/__init__.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:37.956908 seven_cloudapp-1.0.99/seven_cloudapp/handlers/
+-rw-rw-rw-   0        0        0      186 2020-05-26 07:27:31.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:37.972864 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/
+-rw-rw-rw-   0        0        0      260 2020-11-20 08:18:12.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/__init__.py
+-rw-rw-rw-   0        0        0     1479 2020-12-16 09:26:24.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/act.py
+-rw-rw-rw-   0        0        0   411235 2020-11-03 10:29:20.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/address.py
+-rw-rw-rw-   0        0        0     1279 2020-11-20 08:22:54.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/app.py
+-rw-rw-rw-   0        0        0     4024 2020-12-16 09:29:25.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/goods.py
+-rw-rw-rw-   0        0        0      552 2020-11-10 08:02:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/lottery.py
+-rw-rw-rw-   0        0        0     1421 2020-11-24 09:25:14.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/machine.py
+-rw-rw-rw-   0        0        0     9391 2020-12-09 10:28:29.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/prize.py
+-rw-rw-rw-   0        0        0     7943 2020-11-05 09:31:06.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/theme.py
+-rw-rw-rw-   0        0        0     7369 2020-12-16 06:29:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/user.py
+-rw-rw-rw-   0        0        0      546 2020-12-16 02:49:49.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/core.py
+-rw-rw-rw-   0        0        0     1678 2020-09-07 09:02:32.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/monitor.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:37.999792 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/
+-rw-rw-rw-   0        0        0      314 2020-08-12 10:23:42.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/__init__.py
+-rw-rw-rw-   0        0        0    17128 2020-12-16 03:14:58.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/act_s.py
+-rw-rw-rw-   0        0        0    12288 2020-12-10 09:01:19.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/app_s.py
+-rw-rw-rw-   0        0        0     6634 2020-12-16 03:16:15.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/base_s.py
+-rw-rw-rw-   0        0        0     7385 2020-12-16 05:59:06.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/goods_s.py
+-rw-rw-rw-   0        0        0     6229 2020-12-16 03:50:26.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/machine_s.py
+-rw-rw-rw-   0        0        0    19847 2020-12-17 06:29:09.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/order_s.py
+-rw-rw-rw-   0        0        0    10870 2020-12-16 01:42:56.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/price_s.py
+-rw-rw-rw-   0        0        0    14654 2020-12-16 07:12:02.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/prize_s.py
+-rw-rw-rw-   0        0        0    12404 2020-12-10 03:21:07.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/report_s.py
+-rw-rw-rw-   0        0        0     1853 2020-11-04 08:20:01.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/sms_s.py
+-rw-rw-rw-   0        0        0     3481 2020-11-04 08:46:59.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/theme_s.py
+-rw-rw-rw-   0        0        0    15180 2020-12-16 03:22:14.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/throw_s.py
+-rw-rw-rw-   0        0        0    15987 2020-12-17 06:29:12.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/user_s.py
+-rw-rw-rw-   0        0        0    15160 2020-12-16 06:31:36.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/seven_base.py
+-rw-rw-rw-   0        0        0    38605 2020-12-16 05:53:16.000000 seven_cloudapp-1.0.99/seven_cloudapp/handlers/top_base.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.001787 seven_cloudapp-1.0.99/seven_cloudapp/libs/
+-rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.009766 seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/
+-rw-rw-rw-   0        0        0      196 2020-05-26 07:27:31.000000 seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/__init__.py
+-rw-rw-rw-   0        0        0     2812 2020-12-07 08:26:14.000000 seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/oss2help.py
+-rw-rw-rw-   0        0        0     5492 2020-11-24 01:55:28.000000 seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/seven.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.033702 seven_cloudapp-1.0.99/seven_cloudapp/models/
+-rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/__init__.py
+-rw-rw-rw-   0        0        0    11184 2020-12-11 07:06:48.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/behavior_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.035696 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/
+-rw-rw-rw-   0        0        0      141 2020-08-07 10:24:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/__init__.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.042677 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/
+-rw-rw-rw-   0        0        0       62 2020-12-16 10:16:02.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/__init__.py
+-rw-rw-rw-   0        0        0     2679 2020-12-11 07:30:19.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_info_model.py
+-rw-rw-rw-   0        0        0     3508 2020-12-16 10:18:22.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_prize_model.py
+-rw-rw-rw-   0        0        0     2302 2020-12-16 10:14:23.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_type_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.045670 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/app/
+-rw-rw-rw-   0        0        0       26 2020-11-18 02:15:07.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/app/__init__.py
+-rw-rw-rw-   0        0        0     2471 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/app/app_info_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.049659 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/base/
+-rw-rw-rw-   0        0        0       28 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/base/__init__.py
+-rw-rw-rw-   0        0        0     2605 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/base/base_info_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.065616 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/
+-rw-rw-rw-   0        0        0       75 2020-11-18 02:14:40.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/__init__.py
+-rw-rw-rw-   0        0        0     1199 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_log_model.py
+-rw-rw-rw-   0        0        0     1901 2020-12-16 08:51:15.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_orm_model.py
+-rw-rw-rw-   0        0        0     1402 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_report_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.069605 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/browse/
+-rw-rw-rw-   0        0        0       29 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/browse/__init__.py
+-rw-rw-rw-   0        0        0     1281 2020-11-19 06:02:05.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/browse/browse_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.072598 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/coin/
+-rw-rw-rw-   0        0        0       28 2020-11-18 02:14:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/coin/__init__.py
+-rw-rw-rw-   0        0        0     2107 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/coin/coin_order_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.075590 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/collect/
+-rw-rw-rw-   0        0        0       30 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/collect/__init__.py
+-rw-rw-rw-   0        0        0     1287 2020-11-19 05:47:07.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/collect/collect_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.078581 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/consume/
+-rw-rw-rw-   0        0        0       35 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/consume/__init__.py
+-rw-rw-rw-   0        0        0     1245 2020-11-19 09:15:28.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/consume/consume_gear_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.083568 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/
+-rw-rw-rw-   0        0        0       50 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/__init__.py
+-rw-rw-rw-   0        0        0     1369 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/course_info_model.py
+-rw-rw-rw-   0        0        0     1364 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/course_type_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.085563 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/friend/
+-rw-rw-rw-   0        0        0       30 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/friend/__init__.py
+-rw-rw-rw-   0        0        0     1536 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/friend/friend_link_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.089552 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/
+-rw-rw-rw-   0        0        0       45 2020-11-18 02:14:14.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/__init__.py
+-rw-rw-rw-   0        0        0     1482 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/gear_log_model.py
+-rw-rw-rw-   0        0        0     1335 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/gear_value_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.093541 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/invite/
+-rw-rw-rw-   0        0        0       29 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/invite/__init__.py
+-rw-rw-rw-   0        0        0     1370 2020-12-01 03:04:14.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/invite/invite_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.097531 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/login/
+-rw-rw-rw-   0        0        0       27 2020-11-18 02:13:56.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/login/__init__.py
+-rw-rw-rw-   0        0        0     1357 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/login/login_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.103515 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/
+-rw-rw-rw-   0        0        0       56 2020-11-19 08:40:12.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/__init__.py
+-rw-rw-rw-   0        0        0     1192 2020-11-19 08:40:12.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/lottery_log_model.py
+-rw-rw-rw-   0        0        0     2087 2020-12-17 07:20:03.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/lottery_value_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.111493 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/
+-rw-rw-rw-   0        0        0       78 2020-11-18 02:13:15.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/__init__.py
+-rw-rw-rw-   0        0        0     2055 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_info_model.py
+-rw-rw-rw-   0        0        0     1409 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_value_log_model.py
+-rw-rw-rw-   0        0        0     1352 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_value_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.114486 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/marketing/
+-rw-rw-rw-   0        0        0       36 2020-12-16 10:16:21.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/marketing/__init__.py
+-rw-rw-rw-   0        0        0     1490 2020-12-16 10:14:23.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/marketing/marketing_program_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.116480 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/message/
+-rw-rw-rw-   0        0        0       31 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/message/__init__.py
+-rw-rw-rw-   0        0        0     2367 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/message/message_info_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.119472 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/middler/
+-rw-rw-rw-   0        0        0       48 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/middler/__init__.py
+-rw-rw-rw-   0        0        0     1482 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/middler/middler_product_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.122464 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/operation/
+-rw-rw-rw-   0        0        0       31 2020-11-18 02:12:53.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/operation/__init__.py
+-rw-rw-rw-   0        0        0     1891 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/operation/operation_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.129445 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/pay/
+-rw-rw-rw-   0        0        0       27 2020-11-18 02:12:38.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/pay/__init__.py
+-rw-rw-rw-   0        0        0     1960 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/pay/pay_order_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.132438 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/price/
+-rw-rw-rw-   0        0        0       28 2020-11-18 02:12:23.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/price/__init__.py
+-rw-rw-rw-   0        0        0     1318 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/price/price_gear_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.136427 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/
+-rw-rw-rw-   0        0        0       50 2020-11-18 02:10:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/__init__.py
+-rw-rw-rw-   0        0        0     2062 2020-12-11 07:30:19.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/prize_order_model.py
+-rw-rw-rw-   0        0        0     2965 2020-12-15 08:39:02.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/prize_roster_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.140416 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/recommend/
+-rw-rw-rw-   0        0        0       34 2020-11-25 07:07:41.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/recommend/__init__.py
+-rw-rw-rw-   0        0        0     1343 2020-11-25 07:07:41.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/recommend/recommend_goods_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.143408 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/reward/
+-rw-rw-rw-   0        0        0       35 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/reward/__init__.py
+-rw-rw-rw-   0        0        0     1333 2020-11-19 09:15:55.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/reward/reward_order_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.146400 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/signin/
+-rw-rw-rw-   0        0        0       29 2020-11-25 07:21:13.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/signin/__init__.py
+-rw-rw-rw-   0        0        0     1266 2020-11-25 07:21:13.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/signin/signin_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.152384 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/skin/
+-rw-rw-rw-   0        0        0       27 2020-11-18 02:12:03.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/skin/__init__.py
+-rw-rw-rw-   0        0        0     1469 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/skin/skin_info_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.157371 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/
+-rw-rw-rw-   0        0        0       47 2020-11-19 08:12:08.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/__init__.py
+-rw-rw-rw-   0        0        0     1397 2020-11-19 06:09:17.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/task_count_model.py
+-rw-rw-rw-   0        0        0     1436 2020-11-19 06:09:17.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/task_info_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.164353 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/
+-rw-rw-rw-   0        0        0       46 2020-11-18 02:11:52.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/__init__.py
+-rw-rw-rw-   0        0        0     1536 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/theme_info_model.py
+-rw-rw-rw-   0        0        0     1200 2020-11-12 09:11:26.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/theme_ver_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.168342 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/throw/
+-rw-rw-rw-   0        0        0       29 2020-11-18 02:11:35.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/throw/__init__.py
+-rw-rw-rw-   0        0        0     1526 2020-11-12 09:12:11.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/throw/throw_goods_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.177317 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/
+-rw-rw-rw-   0        0        0       75 2020-11-25 09:47:05.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/__init__.py
+-rw-rw-rw-   0        0        0     1688 2020-11-26 07:09:35.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_blacklist_model.py
+-rw-rw-rw-   0        0        0     2374 2020-12-11 09:09:01.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_info_model.py
+-rw-rw-rw-   0        0        0     1405 2020-11-24 11:20:59.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_unbind_log_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:38.181307 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/version/
+-rw-rw-rw-   0        0        0       31 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/version/__init__.py
+-rw-rw-rw-   0        0        0     1488 2020-12-15 08:47:27.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/version/version_info_model.py
+-rw-rw-rw-   0        0        0     2334 2020-12-01 08:22:05.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/enum.py
+-rw-rw-rw-   0        0        0     3159 2020-12-16 01:16:26.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/seven_model.py
+-rw-rw-rw-   0        0        0     1943 2020-08-12 10:23:42.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/taobao_model.py
+-rw-rw-rw-   0        0        0     4048 2020-12-16 06:24:12.000000 seven_cloudapp-1.0.99/seven_cloudapp/models/throw_model.py
+drwxrwxrwx   0        0        0        0 2020-12-17 07:22:37.948928 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/
+-rw-rw-rw-   0        0        0     3839 2020-12-17 07:22:37.000000 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6091 2020-12-17 07:22:37.000000 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-12-17 07:22:37.000000 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2020-12-17 07:22:37.000000 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2020-12-17 07:22:37.000000 seven_cloudapp-1.0.99/seven_cloudapp.egg-info/top_level.txt
```

### Comparing `seven_cloudapp-1.0.98/PKG-INFO` & `seven_cloudapp-1.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seven_cloudapp
-Version: 1.0.98
+Version: 1.0.99
 Summary: seven cloudapp
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: # seven_cloudapp
         
         ## 天志互联Python淘宝云应用框架库
         
-        ### 1.0.98 更新内容
+        ### 1.0.99 更新内容
         * 增加UserListExportHandler
         * 修改UserListHandler
         
         ### 1.0.93 更新内容
         * 更新ActTypeModel、LotteryValueLogModel
         
         ### 1.0.90 更新内容
```

### Comparing `seven_cloudapp-1.0.98/README.md` & `seven_cloudapp-1.0.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # seven_cloudapp
 
 ## 天志互联Python淘宝云应用框架库
 
-### 1.0.98 更新内容
+### 1.0.99 更新内容
 * 增加UserListExportHandler
 * 修改UserListHandler
 
 ### 1.0.93 更新内容
 * 更新ActTypeModel、LotteryValueLogModel
 
 ### 1.0.90 更新内容
```

### Comparing `seven_cloudapp-1.0.98/setup.py` & `seven_cloudapp-1.0.99/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_cloudapp",
-    version="1.0.98",
+    version="1.0.99",
     author="seven",
     author_email="tech@gao7.com",
     description="seven cloudapp",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp.git",
```

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/act.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/act.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/address.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/address.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/app.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/app.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/goods.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/goods.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/lottery.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/lottery.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/machine.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/machine.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/prize.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/prize.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/theme.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/theme.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/client/user.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/client/user.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/core.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/core.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/monitor.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/monitor.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/act_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/act_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/app_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/app_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/base_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/base_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/goods_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/goods_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/machine_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/machine_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/order_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/order_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJingCan
 @Date: 2020-06-02 11:08:39
-@LastEditTime: 2020-12-17 11:20:54
+@LastEditTime: 2020-12-17 14:29:09
 @LastEditors: HuangJingCan
 @Description: 订单相关
 """
 from seven_cloudapp.handlers.seven_base import *
 
 from seven_cloudapp.models.seven_model import *
 
@@ -487,12 +487,12 @@
             result_data.append(data_row)
 
         resource_path = ""
         if result_data:
             path = "temp/" + UUIDHelper.get_uuid() + ".xlsx"
             ExcelHelper.export(result_data, path)
 
-            resource_path = OSS2Helper().upload("", path, config.get("oss_folder"), False)
+            resource_path = OSS2Helper().upload("", path, config.get_value("oss_folder"), False)
 
             os.remove(path)
 
         self.reponse_json_success(resource_path)
```

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/price_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/price_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/prize_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/prize_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/report_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/report_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/sms_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/sms_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/theme_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/theme_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/throw_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/throw_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/server/user_s.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/server/user_s.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """
 @Author: HuangJingCan
 @Date: 2020-05-12 20:04:54
-@LastEditTime: 2020-12-17 11:41:04
+@LastEditTime: 2020-12-17 14:28:53
 @LastEditors: HuangJingCan
 @Description: 用户相关
 """
 from seven_cloudapp.handlers.seven_base import *
 
 from seven_cloudapp.models.seven_model import *
 
@@ -234,15 +234,15 @@
             result_data.append(data_row)
 
         resource_path = ""
         if result_data:
             path = "temp/" + UUIDHelper.get_uuid() + ".xlsx"
             ExcelHelper.export(result_data, path)
 
-            resource_path = OSS2Helper().upload("", path, config.get("oss_folder"), False)
+            resource_path = OSS2Helper().upload("", path, config.get_value("oss_folder"), False)
 
             os.remove(path)
 
         self.reponse_json_success(resource_path)
 
 
 class UserBlackStatusHandler(SevenBaseHandler):
@@ -434,12 +434,12 @@
             result_data.append(data_row)
 
         resource_path = ""
         if result_data:
             path = "temp/" + UUIDHelper.get_uuid() + ".xlsx"
             ExcelHelper.export(result_data, path)
 
-            resource_path = OSS2Helper().upload("", path, "test", False)
+            resource_path = OSS2Helper().upload("", path, config.get_value("oss_folder"), False)
 
             os.remove(path)
 
         self.reponse_json_success(resource_path)
```

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/seven_base.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/seven_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/handlers/top_base.py` & `seven_cloudapp-1.0.99/seven_cloudapp/handlers/top_base.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/oss2help.py` & `seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/oss2help.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/libs/customize/seven.py` & `seven_cloudapp-1.0.99/seven_cloudapp/libs/customize/seven.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/behavior_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/behavior_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_prize_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_prize_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/act/act_type_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/act/act_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/app/app_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/app/app_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/base/base_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/base/base_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_orm_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_orm_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/behavior/behavior_report_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/behavior/behavior_report_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/browse/browse_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/browse/browse_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/coin/coin_order_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/coin/coin_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/collect/collect_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/collect/collect_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/consume/consume_gear_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/consume/consume_gear_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/course_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/course_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/course/course_type_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/course/course_type_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/friend/friend_link_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/friend/friend_link_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/gear_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/gear_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/gear/gear_value_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/gear/gear_value_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/invite/invite_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/invite/invite_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/login/login_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/login/login_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/lottery_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/lottery_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/lottery/lottery_value_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/lottery/lottery_value_log_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,28 +19,29 @@
         super(LotteryValueLog, self).__init__()
         self.id = 0  # id
         self.app_id = ""  # app_id
         self.act_id = 0  # act_id
         self.open_id = ""  # open_id
         self.user_nick = ""  # 用户昵称
         self.log_title = ""  # 标题
+        self.log_desc = ""  # 备注
         self.log_info = ""  # 信息
         self.currency_type = 0  # 抽奖货币类型（0无1次数2积分3价格档位）
         self.source_type = 0  # 来源类型：1-购买2-任务3-手动配置4抽奖
         self.change_type = 0  # 变动类型(来源类型+对用的子类型  如:101下单购买201新人有礼202每日签到301手动增加302手动减少401抽奖增加402抽奖减少)
         self.operate_type = 0  # 操作类型(0累计 1消耗)
         self.current_value = 0  # 改动的值
         self.history_value = 0  # 未变化前用户值
         self.main_pay_order_no = ""  # 淘宝主订单号
         self.operator = ""  # 操作人
         self.create_date = "1900-01-01 00:00:00"  # 创建时间
 
     @classmethod
     def get_field_list(self):
-        return ['id', 'app_id', 'act_id', 'open_id', 'user_nick', 'log_title', 'log_info', 'currency_type', 'source_type', 'change_type', 'operate_type', 'current_value', 'history_value', 'main_pay_order_no', 'operator', 'create_date']
+        return ['id', 'app_id', 'act_id', 'open_id', 'user_nick', 'log_title', 'log_desc', 'log_info', 'currency_type', 'source_type', 'change_type', 'operate_type', 'current_value', 'history_value', 'main_pay_order_no', 'operator', 'create_date']
         
     @classmethod
     def get_primary_key(self):
         return "id"
 
     def __str__(self):
         return "lottery_value_log_tb"
```

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_value_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_value_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/machine/machine_value_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/machine/machine_value_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/marketing/marketing_program_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/marketing/marketing_program_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/message/message_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/message/message_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/middler/middler_product_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/middler/middler_product_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/operation/operation_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/operation/operation_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/pay/pay_order_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/pay/pay_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/price/price_gear_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/price/price_gear_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/prize_order_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/prize_order_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/prize/prize_roster_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/prize/prize_roster_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/recommend/recommend_goods_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/recommend/recommend_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/reward/reward_order_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/reward/reward_order_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/signin/signin_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/signin/signin_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/skin/skin_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/skin/skin_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/task_count_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/task_count_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/task/task_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/task/task_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/theme_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/theme_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/theme/theme_ver_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/theme/theme_ver_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/throw/throw_goods_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/throw/throw_goods_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_blacklist_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_blacklist_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/user/user_unbind_log_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/user/user_unbind_log_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/db_models/version/version_info_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/db_models/version/version_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/enum.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/enum.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/seven_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/seven_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/taobao_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/taobao_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp/models/throw_model.py` & `seven_cloudapp-1.0.99/seven_cloudapp/models/throw_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp.egg-info/PKG-INFO` & `seven_cloudapp-1.0.99/seven_cloudapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seven-cloudapp
-Version: 1.0.98
+Version: 1.0.99
 Summary: seven cloudapp
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: # seven_cloudapp
         
         ## 天志互联Python淘宝云应用框架库
         
-        ### 1.0.98 更新内容
+        ### 1.0.99 更新内容
         * 增加UserListExportHandler
         * 修改UserListHandler
         
         ### 1.0.93 更新内容
         * 更新ActTypeModel、LotteryValueLogModel
         
         ### 1.0.90 更新内容
```

### Comparing `seven_cloudapp-1.0.98/seven_cloudapp.egg-info/SOURCES.txt` & `seven_cloudapp-1.0.99/seven_cloudapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

