# Comparing `tmp/nonebot_bison_migang-0.0.4.tar.gz` & `tmp/nonebot_bison_migang-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_bison_migang-0.0.4.tar", max compression
+gzip compressed data, was "nonebot_bison_migang-0.0.5.tar", max compression
```

## Comparing `nonebot_bison_migang-0.0.4.tar` & `nonebot_bison_migang-0.0.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1066 2023-06-09 07:47:59.942544 nonebot_bison_migang-0.0.4/LICENSE
--rw-r--r--   0        0        0     3873 2023-06-09 07:47:59.942544 nonebot_bison_migang-0.0.4/README.md
--rw-r--r--   0        0        0     1092 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/__init__.py
--rw-r--r--   0        0        0     3556 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/__init__.py
--rw-r--r--   0        0        0     7076 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/api.py
--rw-r--r--   0        0        0        0 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/.gitkeep
--rw-r--r--   0        0        0      559 2023-06-09 07:48:00.554551 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/asset-manifest.json
--rw-r--r--   0        0        0     3585 2023-06-09 07:48:00.550551 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/favicon.ico
--rw-r--r--   0        0        0      691 2023-06-09 07:48:00.634552 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/index.html
--rw-r--r--   0        0        0     4153 2023-06-09 07:48:00.638552 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/logo192.png
--rw-r--r--   0        0        0    12066 2023-06-09 07:48:00.702553 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/logo512.png
--rw-r--r--   0        0        0      492 2023-06-09 07:48:00.706553 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/manifest.json
--rw-r--r--   0        0        0       67 2023-06-09 07:48:00.774554 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/robots.txt
--rw-r--r--   0        0        0   564896 2023-06-09 07:48:00.922556 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css
--rw-r--r--   0        0        0   845815 2023-06-09 07:48:00.858555 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css.map
--rw-r--r--   0        0        0     4619 2023-06-09 07:48:01.006557 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js
--rw-r--r--   0        0        0    10592 2023-06-09 07:48:00.926556 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js.map
--rw-r--r--   0        0        0   851033 2023-06-09 07:48:01.202559 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js
--rw-r--r--   0        0        0     2825 2023-06-09 07:48:00.998557 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js.LICENSE.txt
--rw-r--r--   0        0        0  3743619 2023-06-09 07:48:01.370561 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js.map
--rw-r--r--   0        0        0      505 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/jwt.py
--rw-r--r--   0        0        0      710 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/token_manager.py
--rw-r--r--   0        0        0      838 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/types.py
--rw-r--r--   0        0        0      471 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/apis.py
--rw-r--r--   0        0        0     1830 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/bootstrap.py
--rw-r--r--   0        0        0      118 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/__init__.py
--rw-r--r--   0        0        0     9767 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/config_legacy.py
--rw-r--r--   0        0        0    11781 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/db_config.py
--rw-r--r--   0        0        0     3515 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/db_migration.py
--rw-r--r--   0        0        0     2587 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/db_model.py
--rw-r--r--   0        0        0     1857 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/0571870f5222_init_db.py
--rw-r--r--   0        0        0     1483 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/4a46ba54a3f3_alter_type.py
--rw-r--r--   0        0        0     1038 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/5da28f6facb3_rename_tables.py
--rw-r--r--   0        0        0     1561 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/5f3370328e44_add_time_weight_table.py
--rw-r--r--   0        0        0     1275 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/632b8086bc2b_add_user_target.py
--rw-r--r--   0        0        0     1398 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/67c38b3f39c2_make_user_target_not_nullable.py
--rw-r--r--   0        0        0      949 2023-06-09 07:47:59.950544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/8d3863e9d74b_remove_uid_and_type.py
--rw-r--r--   0        0        0      855 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/a333d6224193_add_last_scheduled_time.py
--rw-r--r--   0        0        0     1540 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/a5466912fad0_map_user.py
--rw-r--r--   0        0        0     2363 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/aceef470d69c_alter_fields_not_null.py
--rw-r--r--   0        0        0     1701 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/bd92923c218f_alter_json_not_null.py
--rw-r--r--   0        0        0     1498 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/c97c445e2bdb_add_constraint.py
--rw-r--r--   0        0        0      112 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/__init__.py
--rw-r--r--   0        0        0      147 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/__init__.py
--rw-r--r--   0        0        0      613 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/base.py
--rw-r--r--   0        0        0     3025 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/v1.py
--rw-r--r--   0        0        0     2621 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/v2.py
--rw-r--r--   0        0        0     2613 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/subs_io.py
--rw-r--r--   0        0        0       85 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/utils.py
--rw-r--r--   0        0        0      152 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config/utils.py
--rw-r--r--   0        0        0    16593 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/config_manager.py
--rw-r--r--   0        0        0      866 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/__init__.py
--rw-r--r--   0        0        0     7915 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/arknights.py
--rw-r--r--   0        0        0    15198 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/bilibili.py
--rw-r--r--   0        0        0     1419 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/ff14.py
--rw-r--r--   0        0        0     6399 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/mcbbsnews.py
--rw-r--r--   0        0        0     4621 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/ncm.py
--rw-r--r--   0        0        0    16381 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/platform.py
--rw-r--r--   0        0        0     1896 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/rss.py
--rw-r--r--   0        0        0     6687 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/platform/weibo.py
--rw-r--r--   0        0        0     1001 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/plugin_config.py
--rw-r--r--   0        0        0       57 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/post/__init__.py
--rw-r--r--   0        0        0     1768 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/post/abstract_post.py
--rw-r--r--   0        0        0     2542 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/post/custom_post.py
--rw-r--r--   0        0        0     5969 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/post/post.py
--rw-r--r--   0        0        0     2281 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/post/templates/custom_post.css
--rw-r--r--   0        0        0       23 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/scheduler/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/scheduler/manager.py
--rw-r--r--   0        0        0     5135 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/scheduler/scheduler.py
--rw-r--r--   0        0        0        0 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/script/__init__.py
--rw-r--r--   0        0        0     5059 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/script/cli.py
--rw-r--r--   0        0        0     3179 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/send.py
--rw-r--r--   0        0        0     1075 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/types.py
--rw-r--r--   0        0        0     3093 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/utils/__init__.py
--rw-r--r--   0        0        0     1236 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/utils/context.py
--rw-r--r--   0        0        0     1049 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/utils/get_bot.py
--rw-r--r--   0        0        0      583 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/utils/http.py
--rw-r--r--   0        0        0      938 2023-06-09 07:47:59.954544 nonebot_bison_migang-0.0.4/nonebot_bison/utils/scheduler_config.py
--rw-r--r--   0        0        0     2440 2023-06-09 07:47:59.958544 nonebot_bison_migang-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5674 1970-01-01 00:00:00.000000 nonebot_bison_migang-0.0.4/setup.py
--rw-r--r--   0        0        0     5485 1970-01-01 00:00:00.000000 nonebot_bison_migang-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-09 10:22:51.957626 nonebot_bison_migang-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3873 2023-06-09 10:22:51.957626 nonebot_bison_migang-0.0.5/README.md
+-rw-r--r--   0        0        0     1092 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/__init__.py
+-rw-r--r--   0        0        0     3556 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/__init__.py
+-rw-r--r--   0        0        0     7076 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/api.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/.gitkeep
+-rw-r--r--   0        0        0      559 2023-06-09 10:22:52.485630 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/asset-manifest.json
+-rw-r--r--   0        0        0     3585 2023-06-09 10:22:52.389628 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/favicon.ico
+-rw-r--r--   0        0        0      691 2023-06-09 10:22:52.445628 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/index.html
+-rw-r--r--   0        0        0     4153 2023-06-09 10:22:52.497634 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/logo192.png
+-rw-r--r--   0        0        0    12066 2023-06-09 10:22:52.545647 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/logo512.png
+-rw-r--r--   0        0        0      492 2023-06-09 10:22:52.553650 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-09 10:22:52.593661 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/robots.txt
+-rw-r--r--   0        0        0   564896 2023-06-09 10:22:52.709694 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css
+-rw-r--r--   0        0        0   845815 2023-06-09 10:22:52.673683 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css.map
+-rw-r--r--   0        0        0     4619 2023-06-09 10:22:52.757707 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js
+-rw-r--r--   0        0        0    10592 2023-06-09 10:22:52.729699 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js.map
+-rw-r--r--   0        0        0   851069 2023-06-09 10:22:52.917752 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js
+-rw-r--r--   0        0        0     2825 2023-06-09 10:22:52.801719 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js.LICENSE.txt
+-rw-r--r--   0        0        0  3744335 2023-06-09 10:22:52.961764 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js.map
+-rw-r--r--   0        0        0      505 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/jwt.py
+-rw-r--r--   0        0        0      710 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/token_manager.py
+-rw-r--r--   0        0        0      838 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/types.py
+-rw-r--r--   0        0        0      471 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/apis.py
+-rw-r--r--   0        0        0     1830 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/bootstrap.py
+-rw-r--r--   0        0        0      118 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/__init__.py
+-rw-r--r--   0        0        0     9767 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/config_legacy.py
+-rw-r--r--   0        0        0    11781 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/db_config.py
+-rw-r--r--   0        0        0     3515 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/db_migration.py
+-rw-r--r--   0        0        0     2587 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/db_model.py
+-rw-r--r--   0        0        0     1857 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/0571870f5222_init_db.py
+-rw-r--r--   0        0        0     1483 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/4a46ba54a3f3_alter_type.py
+-rw-r--r--   0        0        0     1038 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/5da28f6facb3_rename_tables.py
+-rw-r--r--   0        0        0     1561 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/5f3370328e44_add_time_weight_table.py
+-rw-r--r--   0        0        0     1275 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/632b8086bc2b_add_user_target.py
+-rw-r--r--   0        0        0     1398 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/67c38b3f39c2_make_user_target_not_nullable.py
+-rw-r--r--   0        0        0      949 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/8d3863e9d74b_remove_uid_and_type.py
+-rw-r--r--   0        0        0      855 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/a333d6224193_add_last_scheduled_time.py
+-rw-r--r--   0        0        0     1540 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/a5466912fad0_map_user.py
+-rw-r--r--   0        0        0     2363 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/aceef470d69c_alter_fields_not_null.py
+-rw-r--r--   0        0        0     1701 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/bd92923c218f_alter_json_not_null.py
+-rw-r--r--   0        0        0     1498 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/c97c445e2bdb_add_constraint.py
+-rw-r--r--   0        0        0      112 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/__init__.py
+-rw-r--r--   0        0        0      147 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/__init__.py
+-rw-r--r--   0        0        0      613 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/base.py
+-rw-r--r--   0        0        0     3025 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/v1.py
+-rw-r--r--   0        0        0     2621 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/v2.py
+-rw-r--r--   0        0        0     2613 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/subs_io.py
+-rw-r--r--   0        0        0       85 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/utils.py
+-rw-r--r--   0        0        0      152 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config/utils.py
+-rw-r--r--   0        0        0    16593 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/config_manager.py
+-rw-r--r--   0        0        0      866 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/__init__.py
+-rw-r--r--   0        0        0     7915 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/arknights.py
+-rw-r--r--   0        0        0    15198 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/bilibili.py
+-rw-r--r--   0        0        0     1419 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/ff14.py
+-rw-r--r--   0        0        0     6399 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/mcbbsnews.py
+-rw-r--r--   0        0        0     4621 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/ncm.py
+-rw-r--r--   0        0        0    16381 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/platform.py
+-rw-r--r--   0        0        0     1833 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/rss.py
+-rw-r--r--   0        0        0     7887 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/platform/weibo.py
+-rw-r--r--   0        0        0     1001 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/plugin_config.py
+-rw-r--r--   0        0        0       57 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/post/__init__.py
+-rw-r--r--   0        0        0     1768 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/post/abstract_post.py
+-rw-r--r--   0        0        0     2542 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/post/custom_post.py
+-rw-r--r--   0        0        0     5969 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/post/post.py
+-rw-r--r--   0        0        0     2281 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/post/templates/custom_post.css
+-rw-r--r--   0        0        0       23 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/scheduler/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/scheduler/manager.py
+-rw-r--r--   0        0        0     5135 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/scheduler/scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/script/__init__.py
+-rw-r--r--   0        0        0     5059 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/script/cli.py
+-rw-r--r--   0        0        0     3258 2023-06-09 10:22:51.965627 nonebot_bison_migang-0.0.5/nonebot_bison/send.py
+-rw-r--r--   0        0        0     1075 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/types.py
+-rw-r--r--   0        0        0     3093 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/utils/__init__.py
+-rw-r--r--   0        0        0     1236 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/utils/context.py
+-rw-r--r--   0        0        0     1049 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/utils/get_bot.py
+-rw-r--r--   0        0        0      583 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/utils/http.py
+-rw-r--r--   0        0        0      938 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/nonebot_bison/utils/scheduler_config.py
+-rw-r--r--   0        0        0     2456 2023-06-09 10:22:51.969627 nonebot_bison_migang-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5697 1970-01-01 00:00:00.000000 nonebot_bison_migang-0.0.5/setup.py
+-rw-r--r--   0        0        0     5522 1970-01-01 00:00:00.000000 nonebot_bison_migang-0.0.5/PKG-INFO
```

### Comparing `nonebot_bison_migang-0.0.4/LICENSE` & `nonebot_bison_migang-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/README.md` & `nonebot_bison_migang-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/__init__.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/__init__.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/api.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/asset-manifest.json` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/asset-manifest.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7552083333333333%*

 * *Differences: {"'entrypoints'": "{insert: [(1, 'static/js/main.eedccf08.js')], delete: [1]}",*

 * * "'files'": "{'main.js': '/bison/static/js/main.eedccf08.js', 'main.eedccf08.js.map': "*

 * *            "'/bison/static/js/main.eedccf08.js.map', delete: ['main.9854bd98.js.map']}"}*

```diff
@@ -1,15 +1,15 @@
 {
     "entrypoints": [
         "static/css/main.6830c7d7.css",
-        "static/js/main.9854bd98.js"
+        "static/js/main.eedccf08.js"
     ],
     "files": {
         "787.72b3b523.chunk.js.map": "/bison/static/js/787.72b3b523.chunk.js.map",
         "index.html": "/bison/index.html",
         "main.6830c7d7.css.map": "/bison/static/css/main.6830c7d7.css.map",
-        "main.9854bd98.js.map": "/bison/static/js/main.9854bd98.js.map",
         "main.css": "/bison/static/css/main.6830c7d7.css",
-        "main.js": "/bison/static/js/main.9854bd98.js",
+        "main.eedccf08.js.map": "/bison/static/js/main.eedccf08.js.map",
+        "main.js": "/bison/static/js/main.eedccf08.js",
         "static/js/787.72b3b523.chunk.js": "/bison/static/js/787.72b3b523.chunk.js"
     }
 }
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/favicon.ico` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/index.html` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/bison/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/bison/logo192.png"/><link rel="manifest" href="/bison/manifest.json"/><title>Nonebot Bison Migang Admin</title><script defer="defer" src="/bison/static/js/main.9854bd98.js"></script><link href="/bison/static/css/main.6830c7d7.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
+<!doctype html><html lang="en"><head><meta charset="utf-8"/><link rel="icon" href="/bison/favicon.ico"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Web site created using create-react-app"/><link rel="apple-touch-icon" href="/bison/logo192.png"/><link rel="manifest" href="/bison/manifest.json"/><title>Nonebot Bison Migang Admin</title><script defer="defer" src="/bison/static/js/main.eedccf08.js"></script><link href="/bison/static/css/main.6830c7d7.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div></body></html>
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/logo192.png` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/logo192.png`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/logo512.png` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/logo512.png`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css.map` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/css/main.6830c7d7.css.map`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js.map` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/787.72b3b523.chunk.js.map`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see main.9854bd98.js.LICENSE.txt */ ! function() {
+/*! For license information please see main.eedccf08.js.LICENSE.txt */ ! function() {
     var e = {
             5263: function(e, t, n) {
                 var r, o, i = this && this.__generator || function(e, t) {
                         var n, r, o, i, a = {
                             label: 0,
                             sent: function() {
                                 if (1 & o[0]) throw o[1];
@@ -20439,15 +20439,15 @@
                 } else {
                     var f = document.createElement("div");
                     (Lo || document.body).appendChild(f), Ho[o] = {}, Ho[o].pending = new Promise((function(t) {
                         Ur(e.createElement($o, {
                             transitionClassNames: i,
                             transitionTimeout: a,
                             ref: function(e) {
-                                Ho[o].instance = e, n = e.add(r), t(null)
+                                Ho[o] || (Ho[o] = {}), Ho[o].instance = e, n = e.add(r), t(null)
                             }
                         }), f)
                     }))
                 }
                 return function() {
                     var e, t;
                     null === (t = null === (e = Ho[o]) || void 0 === e ? void 0 : e.instance) || void 0 === t || t.remove(n)
@@ -20721,15 +20721,15 @@
                                 l(), ri[r].pending = null
                             })), a
                         }
                         var c = document.createElement("div");
                         return (Jo || document.body).appendChild(c), ri[r] = {}, ri[r].pending = new Promise((function(t) {
                             Ur(e.createElement(n, {
                                 ref: function(e) {
-                                    return ri[r].instance = e, e.add(o), t(null), e
+                                    return ri[r] || (ri[r] = {}), ri[r].instance = e, e.add(o), t(null), e
                                 }
                             }), c)
                         })), ri[r].instance
                     }, n
                 }($r);
             ["info", "success", "error", "warning", "normal"].forEach((function(e) {
                 oi[e] = function(t) {
@@ -41610,8 +41610,8 @@
                         persistor: UC,
                         children: (0, Un.jsx)(cC, {})
                     })
                 })
             })), HC()
         }()
 }();
-//# sourceMappingURL=main.9854bd98.js.map
+//# sourceMappingURL=main.eedccf08.js.map
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js.LICENSE.txt` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/dist/static/js/main.9854bd98.js.map` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/dist/static/js/main.eedccf08.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8567132116004297%*

 * *Differences: {"'file'": "'static/js/main.eedccf08.js'",*

 * * "'mappings'": "';4CAiCYA,EAAAC,+lFCjCZC,EAAAC,GAAA,SAAAH,EAAA,mDAAAG,EAAA,CAAAC,YAAA,kBAAAJ,CAAA,EAAAK,eAAA,kBAAAC,EAAA,EAAAC,0BAAA,kBAAAC,CAAA,EAAAC,WAAA,kBAAAC,EAAA,EAAAC,UAAA,kBAAAC,EAAA,EAAAC,0BAAA,kBAAAC,EAAA,EAAAC,cAAA,kBAAAC,EAAA,EAAAC,eAAA,kBAAAC,CAAA,EAAAC,MAAA,kBAAAC,CAAA,EAAAC,eAAA,kBAAAC,CAAA,EAAAC,aAAA,kBAAAC,EAAA,EAAAC,UAAA,kBAAAC,EAAA,KDiCYzB,EAAAD,IAAAA,EAAA,KACV2B,cAAgB,gBAChB1B,EAAA2B,QAAU,UACV3B,EAAA4B,UAAY,YACZ5B,EAAA6B,SAAW,WEhCN,IAAMC,EAAU,SA […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "static/js/main.9854bd98.js",
+    "file": "static/js/main.eedccf08.js",
     "names": [
         "e",
         "t",
         "m",
         "exports",
         "QueryStatus",
         "buildCreateApi",
@@ -8142,17 +8142,17 @@
         "import _extends from \"@babel/runtime/helpers/extends\";\nimport _defineProperty from \"@babel/runtime/helpers/defineProperty\";\n\nfunction ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) { symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); } keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nimport React, { useContext } from 'react';\nimport { IconContext } from '../context';\n\nfunction IconInfoCircleFillComponent(iconProps, ref) {\n  var _useContext = useContext(IconContext),\n      _useContext$prefixCls = _useContext.prefixCls,\n      prefixCls = _useContext$prefixCls === void 0 ? 'arco' : _useContext$prefixCls;\n\n  var spin = iconProps.spin,\n      className = iconProps.className;\n\n  var props = _objectSpread(_objectSpread({\n    \"aria-hidden\": true,\n    focusable: false,\n    ref: ref\n  }, iconProps), {}, {\n    className: \"\".concat(className ? className + ' ' : '').concat(prefixCls, \"-icon \").concat(prefixCls, \"-icon-info-circle-fill\")\n  });\n\n  if (spin) {\n    props.className = \"\".concat(props.className, \" \").concat(prefixCls, \"-icon-loading\");\n  }\n\n  delete props.spin;\n  delete props.isIcon;\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    fill: \"none\",\n    stroke: \"currentColor\",\n    strokeWidth: \"4\",\n    viewBox: \"0 0 48 48\"\n  }, props), /*#__PURE__*/React.createElement(\"path\", {\n    fill: \"currentColor\",\n    fillRule: \"evenodd\",\n    stroke: \"none\",\n    d: \"M24 44c11.046 0 20-8.954 20-20S35.046 4 24 4 4 12.954 4 24s8.954 20 20 20Zm2-30a1 1 0 0 0-1-1h-2a1 1 0 0 0-1 1v2a1 1 0 0 0 1 1h2a1 1 0 0 0 1-1v-2Zm0 17h1a1 1 0 0 1 1 1v2a1 1 0 0 1-1 1h-6a1 1 0 0 1-1-1v-2a1 1 0 0 1 1-1h1v-8a1 1 0 0 1-1-1v-2a1 1 0 0 1 1-1h3a1 1 0 0 1 1 1v11Z\",\n    clipRule: \"evenodd\"\n  }));\n}\n\nvar IconInfoCircleFill = /*#__PURE__*/React.forwardRef(IconInfoCircleFillComponent);\nIconInfoCircleFill.defaultProps = {\n  isIcon: true\n};\nIconInfoCircleFill.displayName = 'IconInfoCircleFill';\nexport default IconInfoCircleFill;",
         "import _extends from \"@babel/runtime/helpers/extends\";\nimport _defineProperty from \"@babel/runtime/helpers/defineProperty\";\n\nfunction ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) { symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); } keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nimport React, { useContext } from 'react';\nimport { IconContext } from '../context';\n\nfunction IconExclamationCircleFillComponent(iconProps, ref) {\n  var _useContext = useContext(IconContext),\n      _useContext$prefixCls = _useContext.prefixCls,\n      prefixCls = _useContext$prefixCls === void 0 ? 'arco' : _useContext$prefixCls;\n\n  var spin = iconProps.spin,\n      className = iconProps.className;\n\n  var props = _objectSpread(_objectSpread({\n    \"aria-hidden\": true,\n    focusable: false,\n    ref: ref\n  }, iconProps), {}, {\n    className: \"\".concat(className ? className + ' ' : '').concat(prefixCls, \"-icon \").concat(prefixCls, \"-icon-exclamation-circle-fill\")\n  });\n\n  if (spin) {\n    props.className = \"\".concat(props.className, \" \").concat(prefixCls, \"-icon-loading\");\n  }\n\n  delete props.spin;\n  delete props.isIcon;\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    fill: \"none\",\n    stroke: \"currentColor\",\n    strokeWidth: \"4\",\n    viewBox: \"0 0 48 48\"\n  }, props), /*#__PURE__*/React.createElement(\"path\", {\n    fill: \"currentColor\",\n    fillRule: \"evenodd\",\n    stroke: \"none\",\n    d: \"M24 44c11.046 0 20-8.954 20-20S35.046 4 24 4 4 12.954 4 24s8.954 20 20 20Zm-2-11a1 1 0 0 0 1 1h2a1 1 0 0 0 1-1v-2a1 1 0 0 0-1-1h-2a1 1 0 0 0-1 1v2Zm4-18a1 1 0 0 0-1-1h-2a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1h2a1 1 0 0 0 1-1V15Z\",\n    clipRule: \"evenodd\"\n  }));\n}\n\nvar IconExclamationCircleFill = /*#__PURE__*/React.forwardRef(IconExclamationCircleFillComponent);\nIconExclamationCircleFill.defaultProps = {\n  isIcon: true\n};\nIconExclamationCircleFill.displayName = 'IconExclamationCircleFill';\nexport default IconExclamationCircleFill;",
         "import _extends from \"@babel/runtime/helpers/extends\";\nimport _defineProperty from \"@babel/runtime/helpers/defineProperty\";\n\nfunction ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) { symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); } keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nimport React, { useContext } from 'react';\nimport { IconContext } from '../context';\n\nfunction IconLoadingComponent(iconProps, ref) {\n  var _useContext = useContext(IconContext),\n      _useContext$prefixCls = _useContext.prefixCls,\n      prefixCls = _useContext$prefixCls === void 0 ? 'arco' : _useContext$prefixCls;\n\n  var spin = iconProps.spin,\n      className = iconProps.className;\n\n  var props = _objectSpread(_objectSpread({\n    \"aria-hidden\": true,\n    focusable: false,\n    ref: ref\n  }, iconProps), {}, {\n    className: \"\".concat(className ? className + ' ' : '').concat(prefixCls, \"-icon \").concat(prefixCls, \"-icon-loading\")\n  });\n\n  if (spin) {\n    props.className = \"\".concat(props.className, \" \").concat(prefixCls, \"-icon-loading\");\n  }\n\n  delete props.spin;\n  delete props.isIcon;\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    fill: \"none\",\n    stroke: \"currentColor\",\n    strokeWidth: \"4\",\n    viewBox: \"0 0 48 48\"\n  }, props), /*#__PURE__*/React.createElement(\"path\", {\n    d: \"M42 24c0 9.941-8.059 18-18 18S6 33.941 6 24 14.059 6 24 6\"\n  }));\n}\n\nvar IconLoading = /*#__PURE__*/React.forwardRef(IconLoadingComponent);\nIconLoading.defaultProps = {\n  isIcon: true\n};\nIconLoading.displayName = 'IconLoading';\nexport default IconLoading;",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nvar __rest = (this && this.__rest) || function (s, e) {\n    var t = {};\n    for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p) && e.indexOf(p) < 0)\n        t[p] = s[p];\n    if (s != null && typeof Object.getOwnPropertySymbols === \"function\")\n        for (var i = 0, p = Object.getOwnPropertySymbols(s); i < p.length; i++) {\n            if (e.indexOf(p[i]) < 0 && Object.prototype.propertyIsEnumerable.call(s, p[i]))\n                t[p[i]] = s[p[i]];\n        }\n    return t;\n};\nimport React, { useContext } from 'react';\nimport cs from '../_util/classNames';\nimport { ConfigContext } from '../ConfigProvider';\nexport default function IconHover(props) {\n    var _a;\n    var children = props.children, className = props.className, disabled = props.disabled, prefix = props.prefix, _b = props.size, size = _b === void 0 ? 'default' : _b, rest = __rest(props, [\"children\", \"className\", \"disabled\", \"prefix\", \"size\"]);\n    var getPrefixCls = useContext(ConfigContext).getPrefixCls;\n    var prefixCls = getPrefixCls('icon-hover');\n    return (React.createElement(\"span\", __assign({ className: cs(prefixCls, (_a = {},\n            _a[prefix + \"-icon-hover\"] = prefix,\n            _a[prefixCls + \"-size-\" + size] = size && size !== 'default',\n            _a[prefixCls + \"-disabled\"] = disabled,\n            _a), className), onClick: props.onClick }, rest), children));\n}\n",
         "var __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nimport React, { Component } from 'react';\nimport IconClose from '../../icon/react-icon/IconClose';\nimport IconCheckCircleFill from '../../icon/react-icon/IconCheckCircleFill';\nimport IconCloseCircleFill from '../../icon/react-icon/IconCloseCircleFill';\nimport IconInfoCircleFill from '../../icon/react-icon/IconInfoCircleFill';\nimport IconExclamationCircleFill from '../../icon/react-icon/IconExclamationCircleFill';\nimport IconLoading from '../../icon/react-icon/IconLoading';\nimport cs from '../_util/classNames';\nimport IconHover from '../_class/icon-hover';\nimport { IconContext } from '../../icon/react-icon/context';\nvar Notice = /** @class */ (function (_super) {\n    __extends(Notice, _super);\n    function Notice() {\n        var _this = _super !== null && _super.apply(this, arguments) || this;\n        _this.startTimer = function () {\n            var _a = _this.props, duration = _a.duration, onClose = _a.onClose, id = _a.id;\n            // \u81ea\u52a8\u5173\u95ed\n            if (duration !== 0) {\n                _this.timer = window.setTimeout(function () {\n                    onClose && onClose(id);\n                    _this.removeTimer();\n                }, duration);\n            }\n        };\n        _this.removeTimer = function () {\n            if (_this.timer) {\n                window.clearTimeout(_this.timer);\n                _this.timer = null;\n            }\n        };\n        _this.onClose = function () {\n            _this.props.onClose && _this.props.onClose(_this.props.id);\n        };\n        _this.renderIcon = function () {\n            var _a = _this.props, showIcon = _a.showIcon, icon = _a.icon, type = _a.type, prefixCls = _a.prefixCls, iconPrefix = _a.iconPrefix;\n            var content;\n            if (icon) {\n                content = icon;\n            }\n            else if (showIcon) {\n                switch (type) {\n                    case 'info':\n                        content = React.createElement(IconInfoCircleFill, null);\n                        break;\n                    case 'success':\n                        content = React.createElement(IconCheckCircleFill, null);\n                        break;\n                    case 'error':\n                        content = React.createElement(IconCloseCircleFill, null);\n                        break;\n                    case 'warning':\n                        content = React.createElement(IconExclamationCircleFill, null);\n                        break;\n                    case 'loading':\n                        content = React.createElement(IconLoading, null);\n                        break;\n                    default:\n                        break;\n                }\n                content = (React.createElement(IconContext.Provider, { value: iconPrefix ? { prefixCls: iconPrefix } : {} }, content));\n            }\n            return React.createElement(\"span\", { className: prefixCls + \"-icon\" }, content);\n        };\n        _this.onMouseEnter = function () {\n            _this.removeTimer();\n        };\n        _this.onMouseLeave = function () {\n            // An update operation may be triggered after mouseEnter to start a new timer.\n            // mouseEnter(clear) => clickBtn => update(new timer) => mouseLeave\n            _this.removeTimer();\n            _this.startTimer();\n        };\n        return _this;\n    }\n    Notice.prototype.componentDidMount = function () {\n        this.startTimer();\n    };\n    Notice.prototype.componentDidUpdate = function (nextProps) {\n        if (nextProps.duration !== this.props.duration || this.props.update) {\n            this.removeTimer();\n            this.startTimer();\n        }\n    };\n    Notice.prototype.componentWillUnmount = function () {\n        this.removeTimer();\n    };\n    Notice.prototype.render = function () {\n        var _a;\n        var _b = this.props, title = _b.title, content = _b.content, showIcon = _b.showIcon, className = _b.className, style = _b.style, type = _b.type, btn = _b.btn, icon = _b.icon, prefixCls = _b.prefixCls, closable = _b.closable, noticeType = _b.noticeType, iconPrefix = _b.iconPrefix, rtl = _b.rtl;\n        var classNames = cs(prefixCls, prefixCls + \"-\" + type, (_a = {},\n            _a[prefixCls + \"-closable\"] = closable,\n            _a[prefixCls + \"-rtl\"] = rtl,\n            _a), className);\n        var _closable = 'closable' in this.props ? closable : true;\n        var shouldRenderIcon = showIcon;\n        if (type === 'normal' && !icon) {\n            shouldRenderIcon = false;\n        }\n        if (noticeType === 'message') {\n            _closable = closable;\n            return (React.createElement(\"div\", { style: { textAlign: 'center' }, onMouseEnter: this.onMouseEnter, onMouseLeave: this.onMouseLeave },\n                React.createElement(\"div\", { className: classNames, style: style, role: \"alert\" },\n                    shouldRenderIcon && this.renderIcon(),\n                    React.createElement(\"span\", { className: prefixCls + \"-content\" }, content),\n                    _closable && (React.createElement(IconHover, { prefix: prefixCls, className: prefixCls + \"-close-btn\", onClick: this.onClose },\n                        React.createElement(IconClose, null))))));\n        }\n        if (noticeType === 'notification') {\n            return (React.createElement(\"div\", { onMouseEnter: this.onMouseEnter, onMouseLeave: this.onMouseLeave },\n                React.createElement(\"div\", { className: classNames, style: style, role: \"alert\" },\n                    shouldRenderIcon && React.createElement(\"div\", { className: prefixCls + \"-left\" }, this.renderIcon()),\n                    React.createElement(\"div\", { className: prefixCls + \"-right\" },\n                        title && React.createElement(\"div\", { className: prefixCls + \"-title\" }, title),\n                        React.createElement(\"div\", { className: prefixCls + \"-content\" }, content),\n                        btn && React.createElement(\"div\", { className: prefixCls + \"-btn-wrapper\" }, btn)),\n                    _closable && (React.createElement(IconHover, { prefix: prefixCls, className: prefixCls + \"-close-btn\", onClick: this.onClose },\n                        React.createElement(IconContext.Provider, { value: iconPrefix ? { prefixCls: iconPrefix } : {} },\n                            React.createElement(IconClose, null)))))));\n        }\n    };\n    Notice.defaultProps = {\n        type: 'info',\n        showIcon: true,\n        noticeType: 'message',\n        duration: 3000,\n    };\n    return Notice;\n}(Component));\nexport default Notice;\n",
         "var __read = (this && this.__read) || function (o, n) {\n    var m = typeof Symbol === \"function\" && o[Symbol.iterator];\n    if (!m) return o;\n    var i = m.call(o), r, ar = [], e;\n    try {\n        while ((n === void 0 || n-- > 0) && !(r = i.next()).done) ar.push(r.value);\n    }\n    catch (error) { e = { error: error }; }\n    finally {\n        try {\n            if (r && !r.done && (m = i[\"return\"])) m.call(i);\n        }\n        finally { if (e) throw e.error; }\n    }\n    return ar;\n};\nvar __spreadArray = (this && this.__spreadArray) || function (to, from, pack) {\n    if (pack || arguments.length === 2) for (var i = 0, l = from.length, ar; i < l; i++) {\n        if (ar || !(i in from)) {\n            if (!ar) ar = Array.prototype.slice.call(from, 0, i);\n            ar[i] = from[i];\n        }\n    }\n    return to.concat(ar || Array.prototype.slice.call(from));\n};\nimport React, { useState, useImperativeHandle, forwardRef, useContext } from 'react';\nimport { ConfigContext } from '../ConfigProvider';\nvar ContextHolderElement = forwardRef(function (_props, ref) {\n    var configContext = useContext(ConfigContext);\n    var _a = __read(useState([]), 2), instances = _a[0], setInstances = _a[1];\n    function addInstance(ins) {\n        setInstances(function (originInstances) { return __spreadArray(__spreadArray([], __read(originInstances), false), [ins], false); });\n    }\n    function removeInstance(ins) {\n        setInstances(function (originInstances) { return originInstances.filter(function (originIns) { return ins !== originIns; }); });\n    }\n    function getContextConfig() {\n        return configContext;\n    }\n    useImperativeHandle(ref, function () { return ({\n        addInstance: addInstance,\n        removeInstance: removeInstance,\n        getContextConfig: getContextConfig,\n    }); });\n    return (React.createElement(React.Fragment, null, React.Children.map(instances, function (child, index) { return React.cloneElement(child, { key: index }); })));\n});\nexport default ContextHolderElement;\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React, { createRef } from 'react';\nimport ContextHolderElement from '../_util/contextHolder';\nimport Message from '.';\nimport { isString } from '../_util/is';\nfunction useMessage(commonConfig) {\n    if (commonConfig === void 0) { commonConfig = {}; }\n    var maxCount = commonConfig.maxCount, _a = commonConfig.duration, duration = _a === void 0 ? 3000 : _a, _prefixCls = commonConfig.prefixCls;\n    var contextHolderRef = createRef();\n    var holderEle = React.createElement(ContextHolderElement, { ref: contextHolderRef });\n    var messageInstance = {};\n    var notice;\n    function addNotice(config) {\n        var prefixCls, rtl;\n        if (contextHolderRef.current) {\n            var contextConfig = contextHolderRef.current.getContextConfig();\n            rtl = contextConfig.rtl;\n            prefixCls = contextConfig.prefixCls;\n        }\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var _noticeProps = __assign({ position: 'top', duration: duration }, config);\n        var position = _noticeProps.position, transitionClassNames = _noticeProps.transitionClassNames;\n        var id;\n        if (messageInstance[position]) {\n            var notices = messageInstance[position].state.notices;\n            if (notices.length >= maxCount) {\n                var updated = notices[0];\n                id = updated.id;\n                notices.shift();\n                messageInstance[position].add(__assign(__assign({}, _noticeProps), { id: id }));\n            }\n            else {\n                id = messageInstance[position].add(_noticeProps);\n            }\n        }\n        else {\n            notice = (React.createElement(Message, { transitionClassNames: transitionClassNames, ref: function (instance) {\n                    messageInstance[position] = instance;\n                    if (messageInstance[position]) {\n                        id = messageInstance[position].add(_noticeProps);\n                    }\n                }, prefixCls: mergedPrefixCls, rtl: rtl }));\n            contextHolderRef.current.addInstance(notice);\n        }\n        var close = function () {\n            if (messageInstance[position]) {\n                messageInstance[position].remove(id);\n            }\n        };\n        return close;\n    }\n    var messageFuncs = {};\n    ['info', 'success', 'warning', 'error', 'normal'].forEach(function (type) {\n        messageFuncs[type] = function (config) {\n            var _config = isString(config) ? { content: config } : config;\n            return addNotice(__assign(__assign({}, _config), { type: type }));\n        };\n    });\n    return [messageFuncs, holderEle];\n}\nexport default useMessage;\n",
-        "var __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React from 'react';\nimport { CSSTransition, TransitionGroup } from 'react-transition-group';\nimport { render } from '../_util/react-dom';\nimport BaseNotification from '../_class/notification';\nimport Notice from '../_class/notice';\nimport cs from '../_util/classNames';\nimport { isUndefined, isNumber } from '../_util/is';\nimport useMessage from './useMessage';\nvar messageTypes = ['info', 'success', 'error', 'warning', 'loading', 'normal'];\nvar messageInstance = {};\nvar maxCount;\nvar prefixCls;\nvar duration;\nvar container;\nvar rtl;\nfunction addInstance(noticeProps) {\n    var _noticeProps = __assign({ position: 'top', duration: duration }, noticeProps);\n    var position = _noticeProps.position, transitionClassNames = _noticeProps.transitionClassNames, transitionTimeout = _noticeProps.transitionTimeout;\n    var id;\n    var _a = messageInstance[position] || {}, instance = _a.instance, pending = _a.pending;\n    if (instance || pending) {\n        var add_1 = function () {\n            var instance = (messageInstance[position] || {}).instance;\n            var notices = instance.state.notices;\n            if (notices.length >= maxCount) {\n                var updated = notices[0];\n                id = updated.id;\n                notices.shift();\n                instance.add(__assign(__assign({}, _noticeProps), { id: id }));\n            }\n            else {\n                id = instance.add(_noticeProps);\n            }\n        };\n        if (instance) {\n            add_1();\n        }\n        else if (pending === null || pending === void 0 ? void 0 : pending.then) {\n            pending.then(function () {\n                add_1();\n                messageInstance[position].pending = null;\n            });\n        }\n    }\n    else {\n        var div_1 = document.createElement('div');\n        (container || document.body).appendChild(div_1);\n        messageInstance[position] = {};\n        messageInstance[position].pending = new Promise(function (resolve) {\n            render(React.createElement(Message, { transitionClassNames: transitionClassNames, transitionTimeout: transitionTimeout, ref: function (instance) {\n                    messageInstance[position].instance = instance;\n                    id = instance.add(_noticeProps);\n                    resolve(null);\n                } }), div_1);\n        });\n    }\n    var result = function () {\n        var _a, _b;\n        (_b = (_a = messageInstance[position]) === null || _a === void 0 ? void 0 : _a.instance) === null || _b === void 0 ? void 0 : _b.remove(id);\n    };\n    return result;\n}\nvar Message = /** @class */ (function (_super) {\n    __extends(Message, _super);\n    function Message() {\n        var _this = _super !== null && _super.apply(this, arguments) || this;\n        _this.remove = function (id) {\n            var noticeItem = _this.state.notices.find(function (item) { return item.id === id; });\n            if (noticeItem) {\n                _this.update(__assign(__assign({}, noticeItem), { style: __assign(__assign({}, noticeItem.style), { opacity: 0 }) }));\n            }\n            // 100 \u662f\u900f\u660e\u5ea6\u52a8\u753b\u7ed3\u675f\u7684\u65f6\u95f4\n            setTimeout(function () {\n                _super.prototype.remove.call(_this, id);\n            }, 100);\n        };\n        return _this;\n    }\n    Message.prototype.render = function () {\n        var _this = this;\n        var _a = this.props, transitionClassNames = _a.transitionClassNames, _transitionTimeout = _a.transitionTimeout, _prefixCls = _a.prefixCls, _rtl = _a.rtl;\n        var _b = this.state, notices = _b.notices, position = _b.position;\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var mergedRtl = !isUndefined(_rtl) ? _rtl : rtl;\n        var prefixClsMessage = mergedPrefixCls ? mergedPrefixCls + \"-message\" : 'arco-message';\n        var transitionTimeout = {\n            enter: isNumber(_transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.enter) ? _transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.enter : 100,\n            exit: isNumber(_transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.exit) ? _transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.exit : 300,\n        };\n        var classNames = cs(prefixClsMessage + \"-wrapper\", prefixClsMessage + \"-wrapper-\" + position);\n        return (React.createElement(\"div\", { className: classNames },\n            React.createElement(TransitionGroup, { component: null }, notices.map(function (notice) { return (React.createElement(CSSTransition, { key: notice.id, timeout: transitionTimeout, classNames: transitionClassNames || \"fadeMessage\", onExit: function (e) {\n                    e.style.height = e.scrollHeight + \"px\";\n                }, onExiting: function (e) {\n                    e.style.height = 0;\n                }, onExited: function (e) {\n                    e.style.height = 0;\n                    notice.onClose && notice.onClose();\n                } },\n                React.createElement(Notice, __assign({}, notice, { prefixCls: prefixClsMessage, iconPrefix: mergedPrefixCls, onClose: _this.remove, noticeType: \"message\", rtl: mergedRtl })))); }))));\n    };\n    Message.config = function (options) {\n        if (options === void 0) { options = {}; }\n        if (options.maxCount) {\n            maxCount = options.maxCount;\n        }\n        if (options.prefixCls) {\n            prefixCls = options.prefixCls;\n        }\n        if (options.duration) {\n            duration = options.duration;\n        }\n        if (options.rtl) {\n            rtl = options.rtl;\n        }\n        if (options.getContainer && options.getContainer() !== container) {\n            container = options.getContainer();\n            Object.values(messageInstance).forEach(function (_a) {\n                var instance = _a.instance;\n                return instance === null || instance === void 0 ? void 0 : instance.clear();\n            });\n            messageInstance = {};\n        }\n    };\n    Message.clear = function () {\n        Object.values(messageInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.clear();\n        });\n    };\n    Message.addInstance = addInstance;\n    return Message;\n}(BaseNotification));\nmessageTypes.forEach(function (type) {\n    Message[type] = function (noticeProps) {\n        var props = typeof noticeProps === 'string' ? { content: noticeProps } : noticeProps;\n        return addInstance(__assign(__assign({}, props), { type: type }));\n    };\n});\nMessage.useMessage = useMessage;\nexport default Message;\n",
+        "var __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React from 'react';\nimport { CSSTransition, TransitionGroup } from 'react-transition-group';\nimport { render } from '../_util/react-dom';\nimport BaseNotification from '../_class/notification';\nimport Notice from '../_class/notice';\nimport cs from '../_util/classNames';\nimport { isUndefined, isNumber } from '../_util/is';\nimport useMessage from './useMessage';\nvar messageTypes = ['info', 'success', 'error', 'warning', 'loading', 'normal'];\nvar messageInstance = {};\nvar maxCount;\nvar prefixCls;\nvar duration;\nvar container;\nvar rtl;\nfunction addInstance(noticeProps) {\n    var _noticeProps = __assign({ position: 'top', duration: duration }, noticeProps);\n    var position = _noticeProps.position, transitionClassNames = _noticeProps.transitionClassNames, transitionTimeout = _noticeProps.transitionTimeout;\n    var id;\n    var _a = messageInstance[position] || {}, instance = _a.instance, pending = _a.pending;\n    if (instance || pending) {\n        var add_1 = function () {\n            var instance = (messageInstance[position] || {}).instance;\n            var notices = instance.state.notices;\n            if (notices.length >= maxCount) {\n                var updated = notices[0];\n                id = updated.id;\n                notices.shift();\n                instance.add(__assign(__assign({}, _noticeProps), { id: id }));\n            }\n            else {\n                id = instance.add(_noticeProps);\n            }\n        };\n        if (instance) {\n            add_1();\n        }\n        else if (pending === null || pending === void 0 ? void 0 : pending.then) {\n            pending.then(function () {\n                add_1();\n                messageInstance[position].pending = null;\n            });\n        }\n    }\n    else {\n        var div_1 = document.createElement('div');\n        (container || document.body).appendChild(div_1);\n        messageInstance[position] = {};\n        messageInstance[position].pending = new Promise(function (resolve) {\n            render(React.createElement(Message, { transitionClassNames: transitionClassNames, transitionTimeout: transitionTimeout, ref: function (instance) {\n                    if (!messageInstance[position]) {\n                        // getContainer \u53d8\u5316\u65f6\uff0c\u4f1a\u91cd\u7f6e messageInstance\n                        // pending \u4e2d\u7684\u903b\u8f91\u6267\u884c\u665a\u4e8e\u91cd\u7f6e\u903b\u8f91\u65f6\uff0c\u8fd9\u91cc\u9700\u5224\u7a7a\n                        messageInstance[position] = {};\n                    }\n                    messageInstance[position].instance = instance;\n                    id = instance.add(_noticeProps);\n                    resolve(null);\n                } }), div_1);\n        });\n    }\n    var result = function () {\n        var _a, _b;\n        (_b = (_a = messageInstance[position]) === null || _a === void 0 ? void 0 : _a.instance) === null || _b === void 0 ? void 0 : _b.remove(id);\n    };\n    return result;\n}\nvar Message = /** @class */ (function (_super) {\n    __extends(Message, _super);\n    function Message() {\n        var _this = _super !== null && _super.apply(this, arguments) || this;\n        _this.remove = function (id) {\n            var noticeItem = _this.state.notices.find(function (item) { return item.id === id; });\n            if (noticeItem) {\n                _this.update(__assign(__assign({}, noticeItem), { style: __assign(__assign({}, noticeItem.style), { opacity: 0 }) }));\n            }\n            // 100 \u662f\u900f\u660e\u5ea6\u52a8\u753b\u7ed3\u675f\u7684\u65f6\u95f4\n            setTimeout(function () {\n                _super.prototype.remove.call(_this, id);\n            }, 100);\n        };\n        return _this;\n    }\n    Message.prototype.render = function () {\n        var _this = this;\n        var _a = this.props, transitionClassNames = _a.transitionClassNames, _transitionTimeout = _a.transitionTimeout, _prefixCls = _a.prefixCls, _rtl = _a.rtl;\n        var _b = this.state, notices = _b.notices, position = _b.position;\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var mergedRtl = !isUndefined(_rtl) ? _rtl : rtl;\n        var prefixClsMessage = mergedPrefixCls ? mergedPrefixCls + \"-message\" : 'arco-message';\n        var transitionTimeout = {\n            enter: isNumber(_transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.enter) ? _transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.enter : 100,\n            exit: isNumber(_transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.exit) ? _transitionTimeout === null || _transitionTimeout === void 0 ? void 0 : _transitionTimeout.exit : 300,\n        };\n        var classNames = cs(prefixClsMessage + \"-wrapper\", prefixClsMessage + \"-wrapper-\" + position);\n        return (React.createElement(\"div\", { className: classNames },\n            React.createElement(TransitionGroup, { component: null }, notices.map(function (notice) { return (React.createElement(CSSTransition, { key: notice.id, timeout: transitionTimeout, classNames: transitionClassNames || \"fadeMessage\", onExit: function (e) {\n                    e.style.height = e.scrollHeight + \"px\";\n                }, onExiting: function (e) {\n                    e.style.height = 0;\n                }, onExited: function (e) {\n                    e.style.height = 0;\n                    notice.onClose && notice.onClose();\n                } },\n                React.createElement(Notice, __assign({}, notice, { prefixCls: prefixClsMessage, iconPrefix: mergedPrefixCls, onClose: _this.remove, noticeType: \"message\", rtl: mergedRtl })))); }))));\n    };\n    Message.config = function (options) {\n        if (options === void 0) { options = {}; }\n        if (options.maxCount) {\n            maxCount = options.maxCount;\n        }\n        if (options.prefixCls) {\n            prefixCls = options.prefixCls;\n        }\n        if (options.duration) {\n            duration = options.duration;\n        }\n        if (options.rtl) {\n            rtl = options.rtl;\n        }\n        if (options.getContainer && options.getContainer() !== container) {\n            container = options.getContainer();\n            Object.values(messageInstance).forEach(function (_a) {\n                var instance = _a.instance;\n                return instance === null || instance === void 0 ? void 0 : instance.clear();\n            });\n            messageInstance = {};\n        }\n    };\n    Message.clear = function () {\n        Object.values(messageInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.clear();\n        });\n    };\n    Message.addInstance = addInstance;\n    return Message;\n}(BaseNotification));\nmessageTypes.forEach(function (type) {\n    Message[type] = function (noticeProps) {\n        var props = typeof noticeProps === 'string' ? { content: noticeProps } : noticeProps;\n        return addInstance(__assign(__assign({}, props), { type: type }));\n    };\n});\nMessage.useMessage = useMessage;\nexport default Message;\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React, { createRef } from 'react';\nimport ContextHolderElement from '../_util/contextHolder';\nimport Notification from '.';\nimport { isUndefined } from '../_util/is';\nfunction useNotification(commonConfig) {\n    if (commonConfig === void 0) { commonConfig = {}; }\n    var maxCount = commonConfig.maxCount, _a = commonConfig.duration, duration = _a === void 0 ? 3000 : _a, _prefixCls = commonConfig.prefixCls, getContainer = commonConfig.getContainer;\n    var contextHolderRef = createRef();\n    var holderEle = React.createElement(ContextHolderElement, { ref: contextHolderRef });\n    var notificationInstance = {};\n    var notice;\n    function addNotice(noticeProps) {\n        var prefixCls, rtl;\n        if (contextHolderRef.current) {\n            var contextConfig = contextHolderRef.current.getContextConfig();\n            rtl = contextConfig.rtl;\n            prefixCls = contextConfig.prefixCls;\n        }\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var position = noticeProps.position;\n        if (isUndefined(noticeProps.position)) {\n            position = rtl ? 'topLeft' : 'topRight';\n        }\n        var _noticeProps = __assign({ duration: duration }, noticeProps);\n        var id;\n        if (notificationInstance[position]) {\n            var notices = notificationInstance[position].state.notices;\n            if (notices.length >= maxCount) {\n                var updated = notices[0];\n                id = updated.id;\n                notices.shift();\n                notificationInstance[position].add(__assign(__assign({}, _noticeProps), { id: id }));\n            }\n            else {\n                id = notificationInstance[position].add(_noticeProps);\n            }\n        }\n        else {\n            notice = (React.createElement(Notification, { ref: function (instance) {\n                    notificationInstance[position] = instance;\n                    if (notificationInstance[position]) {\n                        id = notificationInstance[position].add(_noticeProps);\n                    }\n                }, prefixCls: mergedPrefixCls, rtl: rtl, getContainer: getContainer }));\n            contextHolderRef.current.addInstance(notice);\n        }\n        return notificationInstance[position];\n    }\n    var notificationFuncs = {};\n    ['info', 'success', 'warning', 'error', 'normal'].forEach(function (type) {\n        notificationFuncs[type] = function (config) {\n            return addNotice(__assign(__assign({}, config), { type: type }));\n        };\n    });\n    return [notificationFuncs, holderEle];\n}\nexport default useNotification;\n",
-        "var __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React from 'react';\nimport { CSSTransition, TransitionGroup } from 'react-transition-group';\nimport { createPortal } from 'react-dom';\nimport { render as ReactDOMRender } from '../_util/react-dom';\nimport BaseNotification from '../_class/notification';\nimport Notice from '../_class/notice';\nimport cs from '../_util/classNames';\nimport { isNumber, isUndefined } from '../_util/is';\nimport useNotification from './useNotification';\nvar notificationTypes = ['info', 'success', 'error', 'warning', 'normal'];\nvar notificationInstance = {};\n// global config\nvar maxCount;\nvar prefixCls;\nvar duration;\nvar container;\nvar rtl;\nvar Notification = /** @class */ (function (_super) {\n    __extends(Notification, _super);\n    function Notification() {\n        var _this = _super !== null && _super.apply(this, arguments) || this;\n        _this.remove = function (id) {\n            var noticeItem = _this.state.notices.find(function (item) { return item.id === id; });\n            if (noticeItem) {\n                _this.update(__assign(__assign({}, noticeItem), { style: __assign(__assign({}, noticeItem.style), { opacity: 0 }) }));\n            }\n            // 200 \u662f\u900f\u660e\u5ea6\u52a8\u753b\u7ed3\u675f\u7684\u65f6\u95f4\n            setTimeout(function () {\n                _super.prototype.remove.call(_this, id);\n            }, 200);\n        };\n        return _this;\n    }\n    Notification.prototype.render = function () {\n        var _a;\n        var _this = this;\n        var notices = this.state.notices;\n        var _b = this.props, _prefixCls = _b.prefixCls, _rtl = _b.rtl, getContainer = _b.getContainer;\n        var position = this.state.position;\n        var mergedRtl = !isUndefined(_rtl) ? _rtl : rtl;\n        if (isUndefined(position)) {\n            position = mergedRtl ? 'topLeft' : 'topRight';\n        }\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var prefixClsNotification = mergedPrefixCls\n            ? mergedPrefixCls + \"-notification\"\n            : 'arco-notification';\n        var transitionClass;\n        if (position === 'topLeft' || position === 'bottomLeft') {\n            transitionClass = 'slideNoticeLeft';\n        }\n        else {\n            transitionClass = 'slideNoticeRight';\n        }\n        var classNames = cs(prefixClsNotification + \"-wrapper\", prefixClsNotification + \"-wrapper-\" + position, (_a = {}, _a[prefixClsNotification + \"-wrapper-rtl\"] = rtl, _a));\n        var container = getContainer === null || getContainer === void 0 ? void 0 : getContainer();\n        var dom = (React.createElement(\"div\", { className: classNames },\n            React.createElement(TransitionGroup, { component: null }, notices.map(function (notice) { return (React.createElement(CSSTransition, { key: notice.id, timeout: {\n                    enter: 400,\n                    exit: 300,\n                }, classNames: transitionClass, onExit: function (e) {\n                    e.style.height = e.scrollHeight + \"px\";\n                }, onExiting: function (e) {\n                    e.style.height = 0;\n                }, onExited: function (e) {\n                    e.style.height = 0;\n                    notice.onClose && notice.onClose();\n                } },\n                React.createElement(Notice, __assign({}, notice, { onClose: _this.remove, prefixCls: prefixClsNotification, iconPrefix: mergedPrefixCls, noticeType: \"notification\", rtl: mergedRtl })))); }))));\n        return container ? createPortal(dom, container) : dom;\n    };\n    Notification.config = function (options) {\n        if (options === void 0) { options = {}; }\n        if (options.maxCount) {\n            maxCount = options.maxCount;\n        }\n        if (options.prefixCls) {\n            prefixCls = options.prefixCls;\n        }\n        if (isNumber(options.duration)) {\n            duration = options.duration;\n        }\n        if (options.rtl) {\n            rtl = options.rtl;\n        }\n        if (options.getContainer && options.getContainer() !== container) {\n            container = options.getContainer();\n            Object.values(notificationInstance).forEach(function (_a) {\n                var notice = _a.instance;\n                return notice === null || notice === void 0 ? void 0 : notice.clear();\n            });\n            notificationInstance = {};\n        }\n    };\n    Notification.clear = function () {\n        Object.values(notificationInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.clear();\n        });\n    };\n    Notification.remove = function (id) {\n        Object.values(notificationInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.remove(id);\n        });\n    };\n    Notification.addInstance = function (noticeProps) {\n        var position = noticeProps.position;\n        if (isUndefined(noticeProps.position)) {\n            position = rtl ? 'topLeft' : 'topRight';\n        }\n        var _noticeProps = __assign({ duration: duration }, noticeProps);\n        var _a = notificationInstance[position] || {}, instance = _a.instance, pending = _a.pending;\n        if (instance || pending) {\n            var add_1 = function () {\n                var instance = (notificationInstance[position] || {}).instance;\n                var notices = instance.state.notices;\n                if (notices.length >= maxCount) {\n                    var updated = notices[0];\n                    notices.shift();\n                    instance.add(__assign(__assign({}, _noticeProps), { id: updated.id }));\n                }\n                else {\n                    instance.add(_noticeProps);\n                }\n                return instance;\n            };\n            if (instance) {\n                add_1();\n            }\n            else if (pending === null || pending === void 0 ? void 0 : pending.then) {\n                pending.then(function () {\n                    add_1();\n                    notificationInstance[position].pending = null;\n                });\n            }\n            return instance;\n        }\n        var div = document.createElement('div');\n        (container || document.body).appendChild(div);\n        notificationInstance[position] = {};\n        notificationInstance[position].pending = new Promise(function (resolve) {\n            ReactDOMRender(React.createElement(Notification, { ref: function (instance) {\n                    notificationInstance[position].instance = instance;\n                    instance.add(_noticeProps);\n                    resolve(null);\n                    return instance;\n                } }), div);\n        });\n        return notificationInstance[position].instance;\n    };\n    return Notification;\n}(BaseNotification));\nnotificationTypes.forEach(function (type) {\n    Notification[type] = function (noticeProps) {\n        return Notification.addInstance(__assign(__assign({}, noticeProps), { type: type }));\n    };\n});\nNotification.useNotification = useNotification;\nexport default Notification;\n",
+        "var __extends = (this && this.__extends) || (function () {\n    var extendStatics = function (d, b) {\n        extendStatics = Object.setPrototypeOf ||\n            ({ __proto__: [] } instanceof Array && function (d, b) { d.__proto__ = b; }) ||\n            function (d, b) { for (var p in b) if (Object.prototype.hasOwnProperty.call(b, p)) d[p] = b[p]; };\n        return extendStatics(d, b);\n    };\n    return function (d, b) {\n        if (typeof b !== \"function\" && b !== null)\n            throw new TypeError(\"Class extends value \" + String(b) + \" is not a constructor or null\");\n        extendStatics(d, b);\n        function __() { this.constructor = d; }\n        d.prototype = b === null ? Object.create(b) : (__.prototype = b.prototype, new __());\n    };\n})();\nvar __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React from 'react';\nimport { CSSTransition, TransitionGroup } from 'react-transition-group';\nimport { createPortal } from 'react-dom';\nimport { render as ReactDOMRender } from '../_util/react-dom';\nimport BaseNotification from '../_class/notification';\nimport Notice from '../_class/notice';\nimport cs from '../_util/classNames';\nimport { isNumber, isUndefined } from '../_util/is';\nimport useNotification from './useNotification';\nvar notificationTypes = ['info', 'success', 'error', 'warning', 'normal'];\nvar notificationInstance = {};\n// global config\nvar maxCount;\nvar prefixCls;\nvar duration;\nvar container;\nvar rtl;\nvar Notification = /** @class */ (function (_super) {\n    __extends(Notification, _super);\n    function Notification() {\n        var _this = _super !== null && _super.apply(this, arguments) || this;\n        _this.remove = function (id) {\n            var noticeItem = _this.state.notices.find(function (item) { return item.id === id; });\n            if (noticeItem) {\n                _this.update(__assign(__assign({}, noticeItem), { style: __assign(__assign({}, noticeItem.style), { opacity: 0 }) }));\n            }\n            // 200 \u662f\u900f\u660e\u5ea6\u52a8\u753b\u7ed3\u675f\u7684\u65f6\u95f4\n            setTimeout(function () {\n                _super.prototype.remove.call(_this, id);\n            }, 200);\n        };\n        return _this;\n    }\n    Notification.prototype.render = function () {\n        var _a;\n        var _this = this;\n        var notices = this.state.notices;\n        var _b = this.props, _prefixCls = _b.prefixCls, _rtl = _b.rtl, getContainer = _b.getContainer;\n        var position = this.state.position;\n        var mergedRtl = !isUndefined(_rtl) ? _rtl : rtl;\n        if (isUndefined(position)) {\n            position = mergedRtl ? 'topLeft' : 'topRight';\n        }\n        var mergedPrefixCls = _prefixCls || prefixCls;\n        var prefixClsNotification = mergedPrefixCls\n            ? mergedPrefixCls + \"-notification\"\n            : 'arco-notification';\n        var transitionClass;\n        if (position === 'topLeft' || position === 'bottomLeft') {\n            transitionClass = 'slideNoticeLeft';\n        }\n        else {\n            transitionClass = 'slideNoticeRight';\n        }\n        var classNames = cs(prefixClsNotification + \"-wrapper\", prefixClsNotification + \"-wrapper-\" + position, (_a = {}, _a[prefixClsNotification + \"-wrapper-rtl\"] = rtl, _a));\n        var container = getContainer === null || getContainer === void 0 ? void 0 : getContainer();\n        var dom = (React.createElement(\"div\", { className: classNames },\n            React.createElement(TransitionGroup, { component: null }, notices.map(function (notice) { return (React.createElement(CSSTransition, { key: notice.id, timeout: {\n                    enter: 400,\n                    exit: 300,\n                }, classNames: transitionClass, onExit: function (e) {\n                    e.style.height = e.scrollHeight + \"px\";\n                }, onExiting: function (e) {\n                    e.style.height = 0;\n                }, onExited: function (e) {\n                    e.style.height = 0;\n                    notice.onClose && notice.onClose();\n                } },\n                React.createElement(Notice, __assign({}, notice, { onClose: _this.remove, prefixCls: prefixClsNotification, iconPrefix: mergedPrefixCls, noticeType: \"notification\", rtl: mergedRtl })))); }))));\n        return container ? createPortal(dom, container) : dom;\n    };\n    Notification.config = function (options) {\n        if (options === void 0) { options = {}; }\n        if (options.maxCount) {\n            maxCount = options.maxCount;\n        }\n        if (options.prefixCls) {\n            prefixCls = options.prefixCls;\n        }\n        if (isNumber(options.duration)) {\n            duration = options.duration;\n        }\n        if (options.rtl) {\n            rtl = options.rtl;\n        }\n        if (options.getContainer && options.getContainer() !== container) {\n            container = options.getContainer();\n            Object.values(notificationInstance).forEach(function (_a) {\n                var notice = _a.instance;\n                return notice === null || notice === void 0 ? void 0 : notice.clear();\n            });\n            notificationInstance = {};\n        }\n    };\n    Notification.clear = function () {\n        Object.values(notificationInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.clear();\n        });\n    };\n    Notification.remove = function (id) {\n        Object.values(notificationInstance).forEach(function (_a) {\n            var instance = _a.instance;\n            instance === null || instance === void 0 ? void 0 : instance.remove(id);\n        });\n    };\n    Notification.addInstance = function (noticeProps) {\n        var position = noticeProps.position;\n        if (isUndefined(noticeProps.position)) {\n            position = rtl ? 'topLeft' : 'topRight';\n        }\n        var _noticeProps = __assign({ duration: duration }, noticeProps);\n        var _a = notificationInstance[position] || {}, instance = _a.instance, pending = _a.pending;\n        if (instance || pending) {\n            var add_1 = function () {\n                var instance = (notificationInstance[position] || {}).instance;\n                var notices = instance.state.notices;\n                if (notices.length >= maxCount) {\n                    var updated = notices[0];\n                    notices.shift();\n                    instance.add(__assign(__assign({}, _noticeProps), { id: updated.id }));\n                }\n                else {\n                    instance.add(_noticeProps);\n                }\n                return instance;\n            };\n            if (instance) {\n                add_1();\n            }\n            else if (pending === null || pending === void 0 ? void 0 : pending.then) {\n                pending.then(function () {\n                    add_1();\n                    notificationInstance[position].pending = null;\n                });\n            }\n            return instance;\n        }\n        var div = document.createElement('div');\n        (container || document.body).appendChild(div);\n        notificationInstance[position] = {};\n        notificationInstance[position].pending = new Promise(function (resolve) {\n            ReactDOMRender(React.createElement(Notification, { ref: function (instance) {\n                    if (!notificationInstance[position]) {\n                        // getContainer \u53d8\u5316\u65f6\uff0c\u4f1a\u91cd\u7f6e notificationInstance\n                        // pending \u4e2d\u7684\u903b\u8f91\u6267\u884c\u665a\u4e8e\u91cd\u7f6e\u903b\u8f91\u65f6\uff0c\u8fd9\u91cc\u9700\u5224\u7a7a\n                        notificationInstance[position] = {};\n                    }\n                    notificationInstance[position].instance = instance;\n                    instance.add(_noticeProps);\n                    resolve(null);\n                    return instance;\n                } }), div);\n        });\n        return notificationInstance[position].instance;\n    };\n    return Notification;\n}(BaseNotification));\nnotificationTypes.forEach(function (type) {\n    Notification[type] = function (noticeProps) {\n        return Notification.addInstance(__assign(__assign({}, noticeProps), { type: type }));\n    };\n});\nNotification.useNotification = useNotification;\nexport default Notification;\n",
         "import _extends from \"@babel/runtime/helpers/extends\";\nimport _defineProperty from \"@babel/runtime/helpers/defineProperty\";\n\nfunction ownKeys(object, enumerableOnly) { var keys = Object.keys(object); if (Object.getOwnPropertySymbols) { var symbols = Object.getOwnPropertySymbols(object); if (enumerableOnly) { symbols = symbols.filter(function (sym) { return Object.getOwnPropertyDescriptor(object, sym).enumerable; }); } keys.push.apply(keys, symbols); } return keys; }\n\nfunction _objectSpread(target) { for (var i = 1; i < arguments.length; i++) { var source = arguments[i] != null ? arguments[i] : {}; if (i % 2) { ownKeys(Object(source), true).forEach(function (key) { _defineProperty(target, key, source[key]); }); } else if (Object.getOwnPropertyDescriptors) { Object.defineProperties(target, Object.getOwnPropertyDescriptors(source)); } else { ownKeys(Object(source)).forEach(function (key) { Object.defineProperty(target, key, Object.getOwnPropertyDescriptor(source, key)); }); } } return target; }\n\nimport React, { useContext } from 'react';\nimport { IconContext } from '../context';\n\nfunction IconEmptyComponent(iconProps, ref) {\n  var _useContext = useContext(IconContext),\n      _useContext$prefixCls = _useContext.prefixCls,\n      prefixCls = _useContext$prefixCls === void 0 ? 'arco' : _useContext$prefixCls;\n\n  var spin = iconProps.spin,\n      className = iconProps.className;\n\n  var props = _objectSpread(_objectSpread({\n    \"aria-hidden\": true,\n    focusable: false,\n    ref: ref\n  }, iconProps), {}, {\n    className: \"\".concat(className ? className + ' ' : '').concat(prefixCls, \"-icon \").concat(prefixCls, \"-icon-empty\")\n  });\n\n  if (spin) {\n    props.className = \"\".concat(props.className, \" \").concat(prefixCls, \"-icon-loading\");\n  }\n\n  delete props.spin;\n  delete props.isIcon;\n  return /*#__PURE__*/React.createElement(\"svg\", _extends({\n    fill: \"none\",\n    stroke: \"currentColor\",\n    strokeWidth: \"4\",\n    viewBox: \"0 0 48 48\"\n  }, props), /*#__PURE__*/React.createElement(\"path\", {\n    d: \"M24 5v6m7 1 4-4m-18 4-4-4m28.5 22H28s-1 3-4 3-4-3-4-3H6.5M40 41H8a2 2 0 0 1-2-2v-8.46a2 2 0 0 1 .272-1.007l6.15-10.54A2 2 0 0 1 14.148 18H33.85a2 2 0 0 1 1.728.992l6.149 10.541A2 2 0 0 1 42 30.541V39a2 2 0 0 1-2 2Z\"\n  }));\n}\n\nvar IconEmpty = /*#__PURE__*/React.forwardRef(IconEmptyComponent);\nIconEmpty.defaultProps = {\n  isIcon: true\n};\nIconEmpty.displayName = 'IconEmpty';\nexport default IconEmpty;",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\n// delete keys from object\nexport default function omit(obj, keys // string \u4e3a\u4e86\u67d0\u4e9b\u6ca1\u6709\u58f0\u660e\u7684\u5c5e\u6027\u88abomit\n) {\n    var clone = __assign({}, obj);\n    keys.forEach(function (key) {\n        if (key in clone) {\n            delete clone[key];\n        }\n    });\n    return clone;\n}\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport { useMemo } from 'react';\nimport omit from '../omit';\nexport default function useMergeProps(componentProps, defaultProps, globalComponentConfig) {\n    var _ignorePropsFromGlobal = componentProps._ignorePropsFromGlobal;\n    var _defaultProps = useMemo(function () {\n        return __assign(__assign({}, defaultProps), (_ignorePropsFromGlobal ? {} : globalComponentConfig));\n    }, [defaultProps, globalComponentConfig, _ignorePropsFromGlobal]);\n    var props = useMemo(function () {\n        // Must remove property of MergePropsOptions before passing it to component\n        var mProps = omit(componentProps, ['_ignorePropsFromGlobal']);\n        // https://github.com/facebook/react/blob/cae635054e17a6f107a39d328649137b83f25972/packages/react/src/ReactElement.js#L312\n        for (var propName in _defaultProps) {\n            if (mProps[propName] === undefined) {\n                mProps[propName] = _defaultProps[propName];\n            }\n        }\n        return mProps;\n    }, [componentProps, _defaultProps]);\n    return props;\n}\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nvar __rest = (this && this.__rest) || function (s, e) {\n    var t = {};\n    for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p) && e.indexOf(p) < 0)\n        t[p] = s[p];\n    if (s != null && typeof Object.getOwnPropertySymbols === \"function\")\n        for (var i = 0, p = Object.getOwnPropertySymbols(s); i < p.length; i++) {\n            if (e.indexOf(p[i]) < 0 && Object.prototype.propertyIsEnumerable.call(s, p[i]))\n                t[p[i]] = s[p[i]];\n        }\n    return t;\n};\nimport React, { memo, useContext, forwardRef } from 'react';\nimport IconEmpty from '../../icon/react-icon/IconEmpty';\nimport cs from '../_util/classNames';\nimport { ConfigContext } from '../ConfigProvider';\nimport useMergeProps from '../_util/hooks/useMergeProps';\nfunction Empty(baseProps, ref) {\n    var _a = useContext(ConfigContext), getPrefixCls = _a.getPrefixCls, globalLocale = _a.locale, componentConfig = _a.componentConfig;\n    var props = useMergeProps(baseProps, {}, componentConfig === null || componentConfig === void 0 ? void 0 : componentConfig.Empty);\n    var style = props.style, className = props.className, description = props.description, icon = props.icon, imgSrc = props.imgSrc, rest = __rest(props, [\"style\", \"className\", \"description\", \"icon\", \"imgSrc\"]);\n    var prefixCls = getPrefixCls('empty');\n    var classNames = cs(prefixCls, className);\n    var noData = globalLocale.Empty.noData;\n    var alt = typeof description === 'string' ? description : 'empty';\n    return (React.createElement(\"div\", __assign({ ref: ref, className: classNames, style: style }, rest),\n        React.createElement(\"div\", { className: prefixCls + \"-wrapper\" },\n            React.createElement(\"div\", { className: prefixCls + \"-image\" }, imgSrc ? React.createElement(\"img\", { alt: alt, src: imgSrc }) : icon || React.createElement(IconEmpty, null)),\n            React.createElement(\"div\", { className: prefixCls + \"-description\" }, description || noData))));\n}\nvar EmptyComponent = forwardRef(Empty);\nEmptyComponent.displayName = 'Empty';\nexport default memo(EmptyComponent);\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nvar configProvider = {};\nexport function setConfigProviderProps(configProviderProps) {\n    configProvider = __assign({}, configProviderProps);\n}\nexport function getConfigProviderProps() {\n    return configProvider;\n}\nvar modalConfig = {\n    simple: true,\n};\nexport var setModalConfig = function (config) {\n    modalConfig = __assign(__assign({}, modalConfig), config);\n};\nexport var getModalConfig = function () {\n    return modalConfig;\n};\nexport var destroyList = [];\n",
         "var __assign = (this && this.__assign) || function () {\n    __assign = Object.assign || function(t) {\n        for (var s, i = 1, n = arguments.length; i < n; i++) {\n            s = arguments[i];\n            for (var p in s) if (Object.prototype.hasOwnProperty.call(s, p))\n                t[p] = s[p];\n        }\n        return t;\n    };\n    return __assign.apply(this, arguments);\n};\nimport React, { useEffect, createContext } from 'react';\nimport defaultLocale from '../locale/default';\nimport { isObject } from '../_util/is';\nimport { lighten } from './util';\nimport Message from '../Message';\nimport Notification from '../Notification';\nimport Empty from '../Empty';\nimport { setConfigProviderProps } from '../Modal/config';\nimport { IconContext } from '../../icon/react-icon/context';\nimport omit from '../_util/omit';\nimport useMergeProps from '../_util/hooks/useMergeProps';\nvar colorList = {\n    primaryColor: {\n        default: '--arcoblue-6',\n        hover: '--arcoblue-5',\n        active: '--arcoblue-7',\n    },\n    successColor: {\n        default: '--green-6',\n        hover: '--green-5',\n        active: '--green-7',\n    },\n    infoColor: {\n        default: '--arcoblue-6',\n        hover: '--arcoblue-5',\n        active: '--arcoblue-7',\n    },\n    warningColor: {\n        default: '--orangered-6',\n        hover: '--orangered-5',\n        active: '--orangered-7',\n    },\n    dangerColor: {\n        default: '--red-6',\n        hover: '--red-5',\n        active: '--red-7',\n    },\n};\nfunction setTheme(theme) {\n    if (theme && isObject(theme)) {\n        var root_1 = document.body;\n        Object.keys(colorList).forEach(function (color) {\n            if (theme[color]) {\n                root_1.style.setProperty(colorList[color].default, lighten(theme[color], 0));\n                if (!theme[color + \"Hover\"]) {\n                    root_1.style.setProperty(colorList[color].hover, lighten(theme[color], 10));\n                }\n                if (!theme[color + \"Active\"]) {\n                    root_1.style.setProperty(colorList[color].active, lighten(theme[color], -10));\n                }\n            }\n        });\n    }\n}\nfunction renderEmpty(componentName) {\n    switch (componentName) {\n        default:\n            return React.createElement(Empty, null);\n    }\n}\nvar defaultProps = {\n    locale: defaultLocale,\n    prefixCls: 'arco',\n    getPopupContainer: function () { return document.body; },\n    size: 'default',\n    renderEmpty: renderEmpty,\n    focusLock: {\n        modal: { autoFocus: true },\n        drawer: { autoFocus: true },\n    },\n};\nvar componentConfig = {};\nexport var ConfigContext = createContext(__assign({ getPrefixCls: function (componentName, customPrefix) {\n        return (customPrefix || 'arco') + \"-\" + componentName;\n    } }, defaultProps));\nfunction ConfigProvider(baseProps) {\n    var props = useMergeProps(baseProps, defaultProps, componentConfig);\n    var theme = props.theme, prefixCls = props.prefixCls, children = props.children, locale = props.locale, rtl = props.rtl, _a = props.effectGlobalNotice, effectGlobalNotice = _a === void 0 ? true : _a;\n    useEffect(function () {\n        setTheme(theme);\n    }, [theme]);\n    useEffect(function () {\n        if (effectGlobalNotice) {\n            Message.config({ prefixCls: prefixCls, rtl: rtl });\n            Notification.config({ prefixCls: prefixCls, rtl: rtl });\n        }\n    }, [prefixCls, rtl, effectGlobalNotice]);\n    function getPrefixCls(componentName, customPrefix) {\n        return (customPrefix || prefixCls) + \"-\" + componentName;\n    }\n    var config = __assign(__assign({}, omit(props, ['children'])), { getPrefixCls: getPrefixCls });\n    useEffect(function () {\n        setConfigProviderProps({ locale: locale, prefixCls: prefixCls, rtl: rtl });\n    }, [locale, prefixCls]);\n    var child = children;\n    if (prefixCls && prefixCls !== 'arco') {\n        child = React.createElement(IconContext.Provider, { value: { prefixCls: prefixCls } }, children);\n    }\n    return React.createElement(ConfigContext.Provider, { value: config }, child);\n}\nConfigProvider.ConfigContext = ConfigContext;\nConfigProvider.displayName = 'ConfigProvider';\nexport default ConfigProvider;\nexport var ConfigConsumer = ConfigContext.Consumer;\n",
         "import React, { useContext, forwardRef } from 'react';\nimport cs from '../_util/classNames';\nimport { ConfigContext } from '../ConfigProvider';\nfunction Typography(props, ref) {\n    var getPrefixCls = useContext(ConfigContext).getPrefixCls;\n    var prefixCls = getPrefixCls('typography');\n    var className = props.className, style = props.style, children = props.children;\n    var classNames = cs(prefixCls, className);\n    return (React.createElement(\"article\", { ref: ref, style: style, className: classNames }, children));\n}\nvar TypographyComponent = forwardRef(Typography);\nTypographyComponent.displayName = 'Typography';\nexport default TypographyComponent;\n",
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/token_manager.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/token_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/admin_page/types.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/admin_page/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/bootstrap.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/config_legacy.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/config_legacy.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/db_config.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/db_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/db_migration.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/db_migration.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/db_model.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/db_model.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/0571870f5222_init_db.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/0571870f5222_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/4a46ba54a3f3_alter_type.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/4a46ba54a3f3_alter_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/5da28f6facb3_rename_tables.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/5da28f6facb3_rename_tables.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/5f3370328e44_add_time_weight_table.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/5f3370328e44_add_time_weight_table.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/632b8086bc2b_add_user_target.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/632b8086bc2b_add_user_target.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/67c38b3f39c2_make_user_target_not_nullable.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/67c38b3f39c2_make_user_target_not_nullable.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/8d3863e9d74b_remove_uid_and_type.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/8d3863e9d74b_remove_uid_and_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/a333d6224193_add_last_scheduled_time.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/a333d6224193_add_last_scheduled_time.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/a5466912fad0_map_user.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/a5466912fad0_map_user.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/aceef470d69c_alter_fields_not_null.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/aceef470d69c_alter_fields_not_null.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/bd92923c218f_alter_json_not_null.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/bd92923c218f_alter_json_not_null.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/migrations/c97c445e2bdb_add_constraint.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/migrations/c97c445e2bdb_add_constraint.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/base.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/v1.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/v1.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/nbesf_model/v2.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/nbesf_model/v2.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config/subs_io/subs_io.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config/subs_io/subs_io.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/config_manager.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/config_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/__init__.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/arknights.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/arknights.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/bilibili.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/ff14.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/ff14.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/mcbbsnews.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/mcbbsnews.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/ncm.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/ncm.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/platform.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/platform.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/rss.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/rss.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         feed = feedparser.parse(res)
         entries = feed.entries
         for entry in entries:
             entry["_target_name"] = feed.feed.title
         return feed.entries
 
     async def parse(self, raw_post: RawPost) -> Post:
-        text = raw_post.get("title", "") + "\n" if raw_post.get("title") else ""
+        text = ""
         soup = bs(raw_post.description, "html.parser")
         text += soup.text.strip()
         pics = list(map(lambda x: x.attrs["src"], soup("img")))
         if raw_post.get("media_content"):
             for media in raw_post["media_content"]:
                 if media.get("medium") == "image" and media.get("url"):
                     pics.append(media.get("url"))
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/platform/weibo.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/platform/weibo.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,38 @@
 import json
 import re
 from collections.abc import Callable
 from datetime import datetime
 from typing import Any, Optional
+from urllib.parse import unquote
 
 from bs4 import BeautifulSoup as bs
 from httpx import AsyncClient
+from lxml import etree
 from nonebot.log import logger
 
 from ..post import Post
 from ..types import *
 from ..utils import SchedulerConfig, http_client
 from .platform import NewMessage
 
+_HEADER = {
+    "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
+    "accept-language": "zh-CN,zh;q=0.9",
+    "authority": "m.weibo.cn",
+    "cache-control": "max-age=0",
+    "sec-fetch-dest": "empty",
+    "sec-fetch-mode": "same-origin",
+    "sec-fetch-site": "same-origin",
+    "upgrade-insecure-requests": "1",
+    "user-agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) "
+    "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.72 "
+    "Mobile Safari/537.36",
+}
+
 
 class WeiboSchedConf(SchedulerConfig):
     name = "weibo.com"
     schedule_type = "interval"
     schedule_setting = {"seconds": 3}
 
 
@@ -121,56 +137,69 @@
         elif raw_post["mblog"].get("pics"):
             return Category(3)
         else:
             return Category(4)
 
     def _get_text(self, raw_text: str) -> str:
         text = raw_text.replace("<br/>", "\n").replace("<br />", "\n")
-        return bs(text, "html.parser").text
+        selector = etree.HTML(text)
+        if selector is None:
+            return text
+        url_elems = selector.xpath("//a[@href]/span[@class='surl-text']")
+        for br in selector.xpath("br"):
+            br.tail = "\n" + br.tail
+        for elem in url_elems:
+            url = elem.getparent().get("href")
+            if (
+                not elem.text.startswith("#")
+                and not elem.text.endswith("#")
+                and (
+                    url.startswith("https://weibo.cn/sinaurl?u=")
+                    or url.startswith("https://video.weibo.com")
+                )
+            ):
+                url = unquote(url.replace("https://weibo.cn/sinaurl?u=", ""))
+                elem.text = f"{elem.text}({url} )"
+        return selector.xpath("string(.)")
+
+    async def _get_long_weibo(self, weibo_id: str) -> dict:
+        try:
+            weibo_info = await self.client.get(
+                "https://m.weibo.cn/statuses/show",
+                params={"id": weibo_id},
+                headers=_HEADER,
+            )
+            weibo_info = weibo_info.json()
+            if not weibo_info or weibo_info["ok"] != 1:
+                return {}
+            return weibo_info["data"]
+        except:
+            logger.info(
+                "detail message error: https://m.weibo.cn/detail/{}".format(weibo_id)
+            )
+        return {}
 
     async def parse(self, raw_post: RawPost) -> Post:
-        header = {
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
-            "accept-language": "zh-CN,zh;q=0.9",
-            "authority": "m.weibo.cn",
-            "cache-control": "max-age=0",
-            "sec-fetch-dest": "empty",
-            "sec-fetch-mode": "same-origin",
-            "sec-fetch-site": "same-origin",
-            "upgrade-insecure-requests": "1",
-            "user-agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) "
-            "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/89.0.4389.72 "
-            "Mobile Safari/537.36",
-        }
         info = raw_post["mblog"]
         retweeted = False
         if info.get("retweeted_status"):
             retweeted = True
-        pic_num = info["retweeted_status"]["pic_num"] if retweeted else info["pic_num"]
-        if info["isLongText"] or pic_num > 9:
-            res = await self.client.get(
-                "https://m.weibo.cn/detail/{}".format(info["mid"]), headers=header
-            )
-            try:
-                match = re.search(r'"status": ([\s\S]+),\s+"call"', res.text)
-                assert match
-                full_json_text = match.group(1)
-                info = json.loads(full_json_text)
-            except:
-                logger.info(
-                    "detail message error: https://m.weibo.cn/detail/{}".format(
-                        info["mid"]
-                    )
-                )
+        if info["isLongText"] or info["pic_num"] > 9:
+            info["text"] = (await self._get_long_weibo(info["mid"]))["text"]
         parsed_text = self._get_text(info["text"])
-        raw_pics_list = (
-            info["retweeted_status"].get("pics", [])
-            if retweeted
-            else info.get("pics", [])
-        )
+        raw_pics_list = info.get("pics", [])
+        if retweeted:
+            retweeted_status = info["retweeted_status"]
+            text = retweeted_status["text"]
+            raw_pics_list = retweeted_status.get("pics", [])
+            if retweeted_status["isLongText"] or retweeted_status["pic_num"] > 9:
+                retweeted_weibo = await self._get_long_weibo(retweeted_status["mid"])
+                text = retweeted_weibo["text"]
+                raw_pics_list = retweeted_weibo.get("pics", [])
+            parsed_text += f"\n=========转发=========\n>>转发@{retweeted_status['user']['screen_name']}\n{self._get_text(text)}"
         pic_urls = [img["large"]["url"] for img in raw_pics_list]
         pics = []
         for pic_url in pic_urls:
             async with http_client(headers={"referer": "https://weibo.com"}) as client:
                 res = await client.get(pic_url)
                 res.raise_for_status()
                 pics.append(res.content)
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/plugin_config.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/plugin_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/post/abstract_post.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/post/abstract_post.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/post/custom_post.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/post/custom_post.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/post/post.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/post/post.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/post/templates/custom_post.css` & `nonebot_bison_migang-0.0.5/nonebot_bison/post/templates/custom_post.css`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/scheduler/manager.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/scheduler/manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/scheduler/scheduler.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/script/cli.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/script/cli.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/send.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/send.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 async def send_msgs(send_target: PlatformTarget, msgs: list[MessageFactory]):
     if not plugin_config.bison_use_pic_merge:
         for msg in msgs:
             await _send_msgs_dispatch(send_target, msg)
         return
     if plugin_config.bison_use_pic_merge == 3:
         # 将文字与图片合成一条消息发送
-        await _send_msgs_dispatch(send_target, MessageFactory(msgs))
+        full_msg = MessageFactory([])
+        for msg in msgs:
+            full_msg += msg
+        await _send_msgs_dispatch(send_target, full_msg)
         return
     msgs = msgs.copy()
     if plugin_config.bison_use_pic_merge == 1:
         await _send_msgs_dispatch(send_target, msgs.pop(0))
     if msgs:
         if len(msgs) == 1:  # 只有一条消息序列就不合并转发
             await _send_msgs_dispatch(send_target, msgs.pop(0))
```

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/types.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/utils/__init__.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/utils/context.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/utils/context.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/utils/get_bot.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/utils/get_bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/utils/http.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/utils/http.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/nonebot_bison/utils/scheduler_config.py` & `nonebot_bison_migang-0.0.5/nonebot_bison/utils/scheduler_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_bison_migang-0.0.4/pyproject.toml` & `nonebot_bison_migang-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-bison-migang"
-version = "0.0.4"
+version = "0.0.5"
 description = "Subscribe message from social medias"
 authors = ["mobai <mobai@mobai.one>"]
 license = "MIT"
 homepage = "https://github.com/LambdaYH/nonebot-bison-migang"
 keywords = ["nonebot", "nonebot2", "qqbot"]
 readme = "README.md"
 packages = [{include = "nonebot_bison"}]
@@ -32,14 +32,15 @@
 pyjwt = "^2.1.0"
 python-socketio = "^5.4.0"
 nonebot-adapter-onebot = "^2.0.0-beta.1"
 nonebot-plugin-htmlrender = ">=0.2.0"
 nonebot-plugin-datastore = "^0.6.2"
 nonebot-plugin-apscheduler = "^0.2.0"
 nonebot-plugin-send-anything-anywhere = "^0.2.6"
+lxml = "^4.9.2"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.4"
 pytest = "^7.0.1"
 pytest-asyncio = "^0.18.1"
 respx = "^0.20.0"
 pytest-cov = "^3.0.0"
```

### Comparing `nonebot_bison_migang-0.0.4/setup.py` & `nonebot_bison_migang-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
  'nonebot_bison.post': ['templates/*']}
 
 install_requires = \
 ['bs4>=0.0.1,<0.0.2',
  'expiringdict>=1.2.1,<2.0.0',
  'feedparser>=6.0.2,<7.0.0',
  'httpx>=0.16.1',
+ 'lxml>=4.9.2,<5.0.0',
  'nonebot-adapter-onebot>=2.0.0-beta.1,<3.0.0',
  'nonebot-plugin-apscheduler>=0.2.0,<0.3.0',
  'nonebot-plugin-datastore>=0.6.2,<0.7.0',
  'nonebot-plugin-htmlrender>=0.2.0',
  'nonebot-plugin-send-anything-anywhere>=0.2.6,<0.3.0',
  'nonebot2>=2.0.0-rc.4,<3.0.0',
  'pillow>=8.1,<10.0',
@@ -38,15 +39,15 @@
  'tinydb>=4.3.0,<5.0.0']
 
 entry_points = \
 {'nb_scripts': ['bison = nonebot_bison.script.cli:main']}
 
 setup_kwargs = {
     'name': 'nonebot-bison-migang',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Subscribe message from social medias',
     'long_description': '<div align="center">\n<h1>Bison </br>通用订阅推送插件</h1>\n\n[![pypi](https://badgen.net/pypi/v/nonebot-bison)](https://pypi.org/project/nonebot-bison/)\n[![license](https://img.shields.io/github/license/felinae98/nonebot-bison)](https://github.com/felinae98/nonebot-bison/blob/main/LICENSE)\n[![action](https://img.shields.io/github/actions/workflow/status/felinae98/nonebot-bison/main.yml?branch=main)](https://github.com/felinae98/nonebot-bison/actions/workflows/main.yml)\n[![docker](https://img.shields.io/docker/image-size/felinae98/nonebot-bison)](https://hub.docker.com/r/felinae98/nonebot-bison)\n[![codecov](https://codecov.io/gh/felinae98/nonebot-bison/branch/main/graph/badge.svg?token=QCFIODJOOA)](https://codecov.io/gh/felinae98/nonebot-bison)\n[![qq group](https://img.shields.io/badge/QQ%E7%BE%A4-868610060-orange)](https://qm.qq.com/cgi-bin/qm/qr?k=pXYMGB_e8b6so3QTqgeV6lkKDtEeYE4f&jump_from=webapi)\n\n[文档](https://nonebot-bison.netlify.app)|[开发文档](https://nonebot-bison.netlify.app/dev)\n\n</div>\n\n## 简介\n\n一款自动爬取各种站点，社交平台更新动态，并将信息推送到 QQ 的机器人。\n基于 [`NoneBot2`](https://github.com/nonebot/nonebot2) 开发（诞生于明日方舟的蹲饼活动）\n\n<details>\n<summary>本项目原名原名nonebot-hk-reporter</summary>\n\n寓意本 Bot 要做全世界跑的最快的搬运机器人，后因名字过于暴力改名\n\n</details>\n本项目名称来源于明日方舟角色拜松——一名龙门的信使，曾经骑自行车追上骑摩托车的德克萨斯\n\n支持的平台：\n\n- 微博\n- Bilibili\n- Bilibili 直播\n- RSS\n- 明日方舟\n- 网易云音乐\n- FF14\n- mcbbs 幻翼块讯\n\n## 功能\n\n- [x] 定时爬取指定网站\n- [x] 通过图片发送文本，防止风控\n- [x] 使用队列限制发送频率\n- [x] 使用网页后台管理 Bot 订阅\n- [ ] 使用可以设置权重的调度器按时间调节不同账号的权重\n\n## 使用方法\n\n**!!注意，如果要使用后台管理功能请使用 pypi 版本或者 docker 版本，如果直接 clone 源代码\n需要按下面方式进行 build**\n\n```bash\ncd ./admin-frontend\npnpm && pnpm run build\n```\n\n可以使用 Docker，docker-compose，作为插件安装在 nonebot 中，或者直接运行\n\n在群里 at Bot 或者直接私聊 Bot “添加订阅”，按照提示输入需要订阅的账号，就可以愉快接收消息了。\n\n参考[文档](https://nonebot-bison.vercel.app/usage/#%E4%BD%BF%E7%94%A8)\n\n## FAQ\n\n1. 报错`TypeError: \'type\' object is not subscriptable`  \n   本项目使用了 Python 3.10 的语法，请将 Python 版本升级到 3.10 及以上，推荐使用 docker 部署\n2. bot 不理我  \n   请确认自己是群主或者管理员，并且检查`COMMAND_START`环境变量是否设为`[""]`\n   或者按照`COMMAND_START`中的设置添加命令前缀，例：\n   `COMMAND_START=["/"]`则应发送`/添加订阅`\n3. 微博漏订阅了\n   微博更新了新的风控措施，某些含有某些关键词的微博会获取不到。\n4. 无法使用后台管理页面\n   1. 确认自己正确配置了 nonebot 的端口，如果在远程或容器外访问网页请确保`HOST=0.0.0.0`\n   2. 确认自己的云服务器的防火墙配置正确\n   3. 确认自己使用了正确的方法安装插件\n\n## 参与开发\n\n欢迎各种 PR，参与开发本插件很简单，只需要对相应平台完成几个接口的编写就行。你只需要一点简单的爬虫知识就行。\n\n如果对整体框架有任何意见或者建议，欢迎 issue。\n\n## 鸣谢\n\n- [`go-cqhttp`](https://github.com/Mrs4s/go-cqhttp)：简单又完善的 cqhttp 实现\n- [`NoneBot2`](https://github.com/nonebot/nonebot2)：超好用的开发框架\n- [`HarukaBot`](https://github.com/SK-415/HarukaBot/): 借鉴了大体的实现思路\n- [`rsshub`](https://github.com/DIYgod/RSSHub)：提供了大量的 api\n\n## License\n\nMIT\n',
     'author': 'mobai',
     'author_email': 'mobai@mobai.one',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/LambdaYH/nonebot-bison-migang',
```

### Comparing `nonebot_bison_migang-0.0.4/PKG-INFO` & `nonebot_bison_migang-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-bison-migang
-Version: 0.0.4
+Version: 0.0.5
 Summary: Subscribe message from social medias
 Home-page: https://github.com/LambdaYH/nonebot-bison-migang
 License: MIT
 Keywords: nonebot,nonebot2,qqbot
 Author: mobai
 Author-email: mobai@mobai.one
 Requires-Python: >=3.10,<4.0.0
@@ -22,14 +22,15 @@
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: yaml
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: expiringdict (>=1.2.1,<2.0.0)
 Requires-Dist: feedparser (>=6.0.2,<7.0.0)
 Requires-Dist: httpx (>=0.16.1)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.0.0-beta.1,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.2.0,<0.3.0)
 Requires-Dist: nonebot-plugin-datastore (>=0.6.2,<0.7.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0)
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.6,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0-rc.4,<3.0.0)
 Requires-Dist: pillow (>=8.1,<10.0)
```
