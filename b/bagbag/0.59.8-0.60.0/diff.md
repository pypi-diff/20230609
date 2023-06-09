# Comparing `tmp/bagbag-0.59.8.tar.gz` & `tmp/bagbag-0.60.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.59.8.tar", max compression
+gzip compressed data, was "bagbag-0.60.0.tar", max compression
```

## Comparing `bagbag-0.59.8.tar` & `bagbag-0.60.0.tar`

### file list

```diff
@@ -1,250 +1,253 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.59.8/LICENSE
--rw-r--r--   0        0        0    16635 2023-05-16 05:51:16.918008 bagbag-0.59.8/README.md
--rw-r--r--   0        0        0     2221 2023-05-16 06:22:37.540609 bagbag-0.59.8/pyproject.toml
--rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.59.8/src/bagbag/Base64/__init__.py
--rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.59.8/src/bagbag/Base64/src.py
--rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.59.8/src/bagbag/Cmd/__init__.py
--rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.59.8/src/bagbag/Cmd/src.py
--rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.59.8/src/bagbag/Cryptoo/__init__.py
--rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.59.8/src/bagbag/Cryptoo/src.py
--rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.59.8/src/bagbag/Funcs/CutSentenceStopWords_src.py
--rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.59.8/src/bagbag/Funcs/CutSentence_src.py
--rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.59.8/src/bagbag/Funcs/FakeIdentity_src.py
--rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.59.8/src/bagbag/Funcs/FileType_src.py
--rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.59.8/src/bagbag/Funcs/Format/__init__.py
--rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.59.8/src/bagbag/Funcs/Format/src.py
--rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.59.8/src/bagbag/Funcs/GetPublicIP_src.py
--rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.59.8/src/bagbag/Funcs/IPAddressConvert_src.py
--rw-r--r--   0        0        0      227 2023-05-12 12:35:25.858029 bagbag-0.59.8/src/bagbag/Funcs/Markdown_src.py
--rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.59.8/src/bagbag/Funcs/Ping_src.py
--rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.59.8/src/bagbag/Funcs/ResizeImage_src.py
--rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.59.8/src/bagbag/Funcs/UUID_src.py
--rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.59.8/src/bagbag/Funcs/Wget_src.py
--rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.59.8/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.59.8/src/bagbag/Hash/__init__.py
--rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.59.8/src/bagbag/Hash/src.py
--rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.59.8/src/bagbag/Http/__init__.py
--rw-r--r--   0        0        0    13440 2023-05-12 12:35:25.862718 bagbag-0.59.8/src/bagbag/Http/src.py
--rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.59.8/src/bagbag/Json/__init__.py
--rw-r--r--   0        0        0     3247 2023-05-16 06:21:45.807910 bagbag-0.59.8/src/bagbag/Json/src.py
--rw-r--r--   0        0        0    10860 2023-05-12 12:35:25.814780 bagbag-0.59.8/src/bagbag/Lg.py
--rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.59.8/src/bagbag/Math/__init__.py
--rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.59.8/src/bagbag/Math/src.py
--rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.59.8/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-15 13:15:56.167334 bagbag-0.59.8/src/bagbag/Os/Path/src.py
--rw-r--r--   0        0        0      831 2023-05-15 13:14:44.707074 bagbag-0.59.8/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     2933 2023-05-12 12:35:25.859730 bagbag-0.59.8/src/bagbag/Os/src.py
--rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.59.8/src/bagbag/Process/__init__.py
--rw-r--r--   0        0        0      985 2023-05-12 12:35:25.864234 bagbag-0.59.8/src/bagbag/Process/src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.59.8/src/bagbag/Python/__init__.py
--rw-r--r--   0        0        0      987 2023-05-12 12:35:25.864640 bagbag-0.59.8/src/bagbag/Python/src.py
--rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.59.8/src/bagbag/Random/__init__.py
--rw-r--r--   0        0        0      633 2023-05-12 12:35:25.865063 bagbag-0.59.8/src/bagbag/Random/src.py
--rw-r--r--   0        0        0      379 2023-05-12 12:35:25.860322 bagbag-0.59.8/src/bagbag/Socket/TCP/__init__.py
--rw-r--r--   0        0        0     4850 2023-05-12 12:35:25.860244 bagbag-0.59.8/src/bagbag/Socket/TCP/src.py
--rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.59.8/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.59.8/src/bagbag/String/__init__.py
--rw-r--r--   0        0        0    16767 2023-05-12 12:35:25.865350 bagbag-0.59.8/src/bagbag/String/src.py
--rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.59.8/src/bagbag/Thread/__init__.py
--rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865712 bagbag-0.59.8/src/bagbag/Thread/src.py
--rw-r--r--   0        0        0      517 2023-05-12 12:35:25.866500 bagbag-0.59.8/src/bagbag/Time/__init__.py
--rw-r--r--   0        0        0     4660 2023-05-12 12:35:25.866441 bagbag-0.59.8/src/bagbag/Time/src.py
--rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.59.8/src/bagbag/Tools/Argparser_src.py
--rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
--rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
--rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    23255 2023-05-12 12:35:25.824849 bagbag-0.59.8/src/bagbag/Tools/BlockChain/Tron/src.py
--rw-r--r--   0        0        0      393 2023-05-12 12:35:25.824665 bagbag-0.59.8/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3094 2023-05-13 07:09:45.206704 bagbag-0.59.8/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.59.8/src/bagbag/Tools/Chan_src.py
--rw-r--r--   0        0        0    32941 2023-05-12 12:35:25.827719 bagbag-0.59.8/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3327 2023-05-12 12:35:25.818786 bagbag-0.59.8/src/bagbag/Tools/Crontab_src.py
--rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.59.8/src/bagbag/Tools/Database/__init__.py
--rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.59.8/src/bagbag/Tools/Database/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.59.8/src/bagbag/Tools/Database/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.59.8/src/bagbag/Tools/Database/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.59.8/src/bagbag/Tools/Database/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.59.8/src/bagbag/Tools/Database/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.59.8/src/bagbag/Tools/Database/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/url.py
--rw-r--r--   0        0        0    33529 2023-05-12 12:35:25.830380 bagbag-0.59.8/src/bagbag/Tools/Database/src.py
--rw-r--r--   0        0        0     5396 2023-05-12 12:35:25.823023 bagbag-0.59.8/src/bagbag/Tools/DistributedLock_src.py
--rw-r--r--   0        0        0     4753 2023-05-12 12:35:25.818559 bagbag-0.59.8/src/bagbag/Tools/Elasticsearch_src.py
--rw-r--r--   0        0        0     4579 2023-05-12 12:35:25.828651 bagbag-0.59.8/src/bagbag/Tools/File_src.py
--rw-r--r--   0        0        0     4502 2023-05-12 12:35:25.820400 bagbag-0.59.8/src/bagbag/Tools/Github_src.py
--rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.59.8/src/bagbag/Tools/JavaScript_src.py
--rw-r--r--   0        0        0     2254 2023-05-12 12:35:25.820526 bagbag-0.59.8/src/bagbag/Tools/Kafka_src.py
--rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.59.8/src/bagbag/Tools/Lock_src.py
--rw-r--r--   0        0        0     6790 2023-05-12 12:35:25.821307 bagbag-0.59.8/src/bagbag/Tools/MatrixBot_src.py
--rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.59.8/src/bagbag/Tools/Nslookup_src.py
--rw-r--r--   0        0        0     2486 2023-05-12 12:35:25.828552 bagbag-0.59.8/src/bagbag/Tools/OCR_src.py
--rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.59.8/src/bagbag/Tools/ProgressBar_src.py
--rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.59.8/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3431 2023-05-12 12:35:25.821880 bagbag-0.59.8/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.59.8/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.59.8/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2724 2023-05-12 12:35:25.820655 bagbag-0.59.8/src/bagbag/Tools/Queue_src.py
--rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.59.8/src/bagbag/Tools/RSS/Feed.py
--rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.59.8/src/bagbag/Tools/RSS/Opml.py
--rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.59.8/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.59.8/src/bagbag/Tools/Ratelimit_src.py
--rw-r--r--   0        0        0    18584 2023-05-12 12:35:25.815203 bagbag-0.59.8/src/bagbag/Tools/Redis_src.py
--rw-r--r--   0        0        0     5565 2023-05-12 12:35:25.820157 bagbag-0.59.8/src/bagbag/Tools/SSH_src.py
--rw-r--r--   0        0        0    31923 2023-05-12 12:35:25.815789 bagbag-0.59.8/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.59.8/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.59.8/src/bagbag/Tools/TelegramBotOfficial_src.py
--rw-r--r--   0        0        0     3269 2023-05-12 12:35:25.828367 bagbag-0.59.8/src/bagbag/Tools/TelegramBot_src.py
--rw-r--r--   0        0        0    24585 2023-05-12 12:35:25.815503 bagbag-0.59.8/src/bagbag/Tools/Telegram_src.py
--rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.59.8/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.59.8/src/bagbag/Tools/Translater_src.py
--rw-r--r--   0        0        0     9678 2023-05-12 12:35:25.823235 bagbag-0.59.8/src/bagbag/Tools/Twitter/Elevated.py
--rw-r--r--   0        0        0     2079 2023-05-12 12:35:25.823650 bagbag-0.59.8/src/bagbag/Tools/Twitter/Essential.py
--rw-r--r--   0        0        0      176 2023-05-12 12:35:25.823540 bagbag-0.59.8/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.59.8/src/bagbag/Tools/URL_src.py
--rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.59.8/src/bagbag/Tools/WaitGroup_src.py
--rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.59.8/src/bagbag/Tools/WebCrawler_src.py
--rw-r--r--   0        0        0     5572 2023-05-12 12:35:25.818682 bagbag-0.59.8/src/bagbag/Tools/WebServer_src.py
--rw-r--r--   0        0        0     1702 2023-05-12 12:35:25.819763 bagbag-0.59.8/src/bagbag/Tools/XPath_src.py
--rw-r--r--   0        0        0     3229 2023-05-12 12:35:25.819187 bagbag-0.59.8/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     3445 2023-05-15 05:44:24.522431 bagbag-0.59.8/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0     4448 2023-05-12 12:35:25.861078 bagbag-0.59.8/src/bagbag/__init__.py
--rw-r--r--   0        0        0    19479 1970-01-01 00:00:00.000000 bagbag-0.59.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.60.0/LICENSE
+-rw-r--r--   0        0        0    16635 2023-05-16 05:51:16.918008 bagbag-0.60.0/README.md
+-rw-r--r--   0        0        0     2244 2023-06-09 06:24:05.692976 bagbag-0.60.0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.60.0/src/bagbag/Base64/__init__.py
+-rw-r--r--   0        0        0      478 2023-05-12 12:35:25.861258 bagbag-0.60.0/src/bagbag/Base64/src.py
+-rw-r--r--   0        0        0      499 2023-05-12 12:35:25.861846 bagbag-0.60.0/src/bagbag/Cmd/__init__.py
+-rw-r--r--   0        0        0     5769 2023-05-12 12:35:25.861768 bagbag-0.60.0/src/bagbag/Cmd/src.py
+-rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.60.0/src/bagbag/Cryptoo/__init__.py
+-rw-r--r--   0        0        0     2538 2023-05-12 12:35:25.866065 bagbag-0.60.0/src/bagbag/Cryptoo/src.py
+-rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.60.0/src/bagbag/File/__init__.py
+-rw-r--r--   0        0        0     4645 2023-06-02 17:04:32.821610 bagbag-0.60.0/src/bagbag/File/src.py
+-rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.60.0/src/bagbag/Funcs/CutSentenceStopWords_src.py
+-rw-r--r--   0        0        0      856 2023-05-12 12:35:25.857574 bagbag-0.60.0/src/bagbag/Funcs/CutSentence_src.py
+-rw-r--r--   0        0        0     6832 2023-05-12 12:35:25.858214 bagbag-0.60.0/src/bagbag/Funcs/FakeIdentity_src.py
+-rw-r--r--   0        0        0      557 2023-05-12 12:35:25.858120 bagbag-0.60.0/src/bagbag/Funcs/FileType_src.py
+-rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.60.0/src/bagbag/Funcs/Format/__init__.py
+-rw-r--r--   0        0        0      836 2023-05-12 12:35:25.858411 bagbag-0.60.0/src/bagbag/Funcs/Format/src.py
+-rw-r--r--   0        0        0      752 2023-05-12 12:35:25.857431 bagbag-0.60.0/src/bagbag/Funcs/GetPublicIP_src.py
+-rw-r--r--   0        0        0      295 2023-05-12 12:35:25.857294 bagbag-0.60.0/src/bagbag/Funcs/IPAddressConvert_src.py
+-rw-r--r--   0        0        0      227 2023-05-12 12:35:25.858029 bagbag-0.60.0/src/bagbag/Funcs/Markdown_src.py
+-rw-r--r--   0        0        0      995 2023-05-12 12:35:25.857504 bagbag-0.60.0/src/bagbag/Funcs/Ping_src.py
+-rw-r--r--   0        0        0     1729 2023-05-12 12:35:25.857363 bagbag-0.60.0/src/bagbag/Funcs/ResizeImage_src.py
+-rw-r--r--   0        0        0      112 2023-05-12 12:35:25.857802 bagbag-0.60.0/src/bagbag/Funcs/UUID_src.py
+-rw-r--r--   0        0        0     1457 2023-05-12 12:35:25.857646 bagbag-0.60.0/src/bagbag/Funcs/Wget_src.py
+-rw-r--r--   0        0        0     1120 2023-05-12 12:35:25.857201 bagbag-0.60.0/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.60.0/src/bagbag/Hash/__init__.py
+-rw-r--r--   0        0        0     1450 2023-05-12 12:35:25.862230 bagbag-0.60.0/src/bagbag/Hash/src.py
+-rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.60.0/src/bagbag/Http/__init__.py
+-rw-r--r--   0        0        0    13444 2023-05-16 06:55:50.470768 bagbag-0.60.0/src/bagbag/Http/src.py
+-rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.60.0/src/bagbag/Json/__init__.py
+-rw-r--r--   0        0        0     3271 2023-05-16 06:24:06.059824 bagbag-0.60.0/src/bagbag/Json/src.py
+-rw-r--r--   0        0        0    10860 2023-06-01 07:11:48.733272 bagbag-0.60.0/src/bagbag/Lg.py
+-rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.60.0/src/bagbag/Math/__init__.py
+-rw-r--r--   0        0        0     2075 2023-05-12 12:35:25.863776 bagbag-0.60.0/src/bagbag/Math/src.py
+-rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.60.0/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-15 13:15:56.167334 bagbag-0.60.0/src/bagbag/Os/Path/src.py
+-rw-r--r--   0        0        0      859 2023-05-16 12:14:50.048628 bagbag-0.60.0/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     2933 2023-05-12 12:35:25.859730 bagbag-0.60.0/src/bagbag/Os/src.py
+-rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.60.0/src/bagbag/Process/__init__.py
+-rw-r--r--   0        0        0      958 2023-06-01 07:09:48.165713 bagbag-0.60.0/src/bagbag/Process/src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.864721 bagbag-0.60.0/src/bagbag/Python/__init__.py
+-rw-r--r--   0        0        0      987 2023-05-12 12:35:25.864640 bagbag-0.60.0/src/bagbag/Python/src.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.60.0/src/bagbag/Random/__init__.py
+-rw-r--r--   0        0        0      700 2023-06-01 06:55:49.958227 bagbag-0.60.0/src/bagbag/Random/src.py
+-rw-r--r--   0        0        0      379 2023-05-12 12:35:25.860322 bagbag-0.60.0/src/bagbag/Socket/TCP/__init__.py
+-rw-r--r--   0        0        0     4850 2023-05-12 12:35:25.860244 bagbag-0.60.0/src/bagbag/Socket/TCP/src.py
+-rw-r--r--   0        0        0       17 2023-05-12 12:35:25.860105 bagbag-0.60.0/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.60.0/src/bagbag/String/__init__.py
+-rw-r--r--   0        0        0    16761 2023-06-01 06:54:57.084155 bagbag-0.60.0/src/bagbag/String/src.py
+-rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.60.0/src/bagbag/Thread/__init__.py
+-rw-r--r--   0        0        0      437 2023-06-01 07:09:39.456063 bagbag-0.60.0/src/bagbag/Thread/src.py
+-rw-r--r--   0        0        0      517 2023-05-12 12:35:25.866500 bagbag-0.60.0/src/bagbag/Time/__init__.py
+-rw-r--r--   0        0        0     4808 2023-06-01 06:54:12.063641 bagbag-0.60.0/src/bagbag/Time/src.py
+-rw-r--r--   0        0        0     2449 2023-05-12 12:35:25.818366 bagbag-0.60.0/src/bagbag/Tools/Argparser_src.py
+-rw-r--r--   0        0        0     2613 2023-05-12 12:35:25.825531 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
+-rw-r--r--   0        0        0      972 2023-05-12 12:35:25.826332 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
+-rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      325 2023-05-12 12:35:25.827344 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    23255 2023-05-12 12:35:25.824849 bagbag-0.60.0/src/bagbag/Tools/BlockChain/Tron/src.py
+-rw-r--r--   0        0        0      393 2023-05-12 12:35:25.824665 bagbag-0.60.0/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3277 2023-06-05 15:36:04.503828 bagbag-0.60.0/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     4615 2023-06-09 06:22:43.542806 bagbag-0.60.0/src/bagbag/Tools/Cache.py
+-rw-r--r--   0        0        0     3886 2023-05-12 12:35:25.816327 bagbag-0.60.0/src/bagbag/Tools/Chan_src.py
+-rw-r--r--   0        0        0    32941 2023-05-29 11:13:19.619696 bagbag-0.60.0/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3238 2023-05-29 11:10:20.747420 bagbag-0.60.0/src/bagbag/Tools/Crontab_src.py
+-rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.60.0/src/bagbag/Tools/Database/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.60.0/src/bagbag/Tools/Database/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.60.0/src/bagbag/Tools/Database/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.60.0/src/bagbag/Tools/Database/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.60.0/src/bagbag/Tools/Database/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.60.0/src/bagbag/Tools/Database/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.60.0/src/bagbag/Tools/Database/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/url.py
+-rw-r--r--   0        0        0    33340 2023-05-17 12:21:58.241698 bagbag-0.60.0/src/bagbag/Tools/Database/src.py
+-rw-r--r--   0        0        0     5250 2023-05-29 11:10:33.731697 bagbag-0.60.0/src/bagbag/Tools/DistributedLock_src.py
+-rw-r--r--   0        0        0     4674 2023-05-29 11:10:40.751258 bagbag-0.60.0/src/bagbag/Tools/Elasticsearch_src.py
+-rw-r--r--   0        0        0     4312 2023-05-29 11:10:51.912539 bagbag-0.60.0/src/bagbag/Tools/Github_src.py
+-rw-r--r--   0        0        0     1451 2023-05-12 12:35:25.827625 bagbag-0.60.0/src/bagbag/Tools/JavaScript_src.py
+-rw-r--r--   0        0        0     8602 2023-06-08 12:22:45.677659 bagbag-0.60.0/src/bagbag/Tools/Kafka_src.py
+-rw-r--r--   0        0        0     2028 2023-05-12 12:35:25.815942 bagbag-0.60.0/src/bagbag/Tools/Lock_src.py
+-rw-r--r--   0        0        0     6634 2023-05-29 11:11:12.945317 bagbag-0.60.0/src/bagbag/Tools/MatrixBot_src.py
+-rw-r--r--   0        0        0      466 2023-05-12 12:35:25.821432 bagbag-0.60.0/src/bagbag/Tools/Nslookup_src.py
+-rw-r--r--   0        0        0     2364 2023-05-29 11:11:50.231133 bagbag-0.60.0/src/bagbag/Tools/OCR_src.py
+-rw-r--r--   0        0        0     2816 2023-05-12 12:35:25.815348 bagbag-0.60.0/src/bagbag/Tools/ProgressBar_src.py
+-rw-r--r--   0        0        0     1660 2023-05-12 12:35:25.821643 bagbag-0.60.0/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3337 2023-06-07 15:52:43.922791 bagbag-0.60.0/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0      127 2023-05-12 12:35:25.821766 bagbag-0.60.0/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4670 2023-05-12 12:35:25.821993 bagbag-0.60.0/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2607 2023-05-29 11:12:14.997684 bagbag-0.60.0/src/bagbag/Tools/Queue_src.py
+-rw-r--r--   0        0        0     2490 2023-05-12 12:35:25.821196 bagbag-0.60.0/src/bagbag/Tools/RSS/Feed.py
+-rw-r--r--   0        0        0      661 2023-05-12 12:35:25.820920 bagbag-0.60.0/src/bagbag/Tools/RSS/Opml.py
+-rw-r--r--   0        0        0      119 2023-05-12 12:35:25.821062 bagbag-0.60.0/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3688 2023-05-12 12:35:25.816210 bagbag-0.60.0/src/bagbag/Tools/Ratelimit_src.py
+-rw-r--r--   0        0        0    18451 2023-05-29 11:12:03.251797 bagbag-0.60.0/src/bagbag/Tools/Redis_src.py
+-rw-r--r--   0        0        0     5565 2023-05-12 12:35:25.820157 bagbag-0.60.0/src/bagbag/Tools/SSH_src.py
+-rw-r--r--   0        0        0    34161 2023-06-06 10:04:38.686181 bagbag-0.60.0/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    14131 2023-05-12 12:35:25.820287 bagbag-0.60.0/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     5111 2023-05-12 12:35:25.816456 bagbag-0.60.0/src/bagbag/Tools/TelegramBotOfficial_src.py
+-rw-r--r--   0        0        0     3068 2023-05-29 11:09:17.718502 bagbag-0.60.0/src/bagbag/Tools/TelegramBot_src.py
+-rw-r--r--   0        0        0    24294 2023-06-06 10:04:52.911244 bagbag-0.60.0/src/bagbag/Tools/Telegram_src.py
+-rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.60.0/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     4276 2023-05-12 12:35:25.819888 bagbag-0.60.0/src/bagbag/Tools/Translater_src.py
+-rw-r--r--   0        0        0     6622 2023-06-06 11:56:02.475141 bagbag-0.60.0/src/bagbag/Tools/Twitter/Browser_src.py
+-rw-r--r--   0        0        0    10901 2023-05-26 13:41:17.507212 bagbag-0.60.0/src/bagbag/Tools/Twitter/Elevated_src.py
+-rw-r--r--   0        0        0     2093 2023-05-26 13:18:47.657372 bagbag-0.60.0/src/bagbag/Tools/Twitter/Essential_src.py
+-rw-r--r--   0        0        0      734 2023-05-31 12:20:33.407553 bagbag-0.60.0/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0     3122 2023-05-12 12:35:25.816080 bagbag-0.60.0/src/bagbag/Tools/URL_src.py
+-rw-r--r--   0        0        0      767 2023-05-12 12:35:25.818906 bagbag-0.60.0/src/bagbag/Tools/WaitGroup_src.py
+-rw-r--r--   0        0        0     8126 2023-05-12 12:35:25.828462 bagbag-0.60.0/src/bagbag/Tools/WebCrawler_src.py
+-rw-r--r--   0        0        0     5572 2023-05-12 12:35:25.818682 bagbag-0.60.0/src/bagbag/Tools/WebServer_src.py
+-rw-r--r--   0        0        0     1702 2023-05-12 12:35:25.819763 bagbag-0.60.0/src/bagbag/Tools/XPath_src.py
+-rw-r--r--   0        0        0     3235 2023-05-16 08:49:31.768572 bagbag-0.60.0/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     3486 2023-06-09 06:19:17.462688 bagbag-0.60.0/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0     4539 2023-06-02 17:02:49.981618 bagbag-0.60.0/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    19515 1970-01-01 00:00:00.000000 bagbag-0.60.0/PKG-INFO
```

### Comparing `bagbag-0.59.8/LICENSE` & `bagbag-0.60.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/README.md` & `bagbag-0.60.0/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/pyproject.toml` & `bagbag-0.60.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.59.8"
+version = "0.60.0"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
@@ -87,14 +87,15 @@
 opencv-python = ">=4.6.0.66"
 tld = ">=0.13"
 matplotlib = ">=3.7.1"
 msgpack = ">=1.0.4"
 psutil = ">=5.9.1"
 lazy-imports = ">=0.3.1"
 html-to-json = ">=2.0.0"
+cachetools = ">=4.2.4"
 
 # 额外的, 为了方便, 但是这个包里面没用到
 
 
 # orator 
 # Fix bug in mysql8.0: https://github.com/sdispater/orator/issues/361
 backpack = ">=0.1"
```

### Comparing `bagbag-0.59.8/src/bagbag/Cmd/src.py` & `bagbag-0.60.0/src/bagbag/Cmd/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Cryptoo/src.py` & `bagbag-0.60.0/src/bagbag/Cryptoo/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/CutSentenceStopWords_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/CutSentenceStopWords_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/CutSentence_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/CutSentence_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/FakeIdentity_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/FakeIdentity_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/FileType_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/FileType_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/Format/src.py` & `bagbag-0.60.0/src/bagbag/Funcs/Format/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/GetPublicIP_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/GetPublicIP_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/Ping_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/Ping_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/ResizeImage_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/ResizeImage_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/Wget_src.py` & `bagbag-0.60.0/src/bagbag/Funcs/Wget_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Funcs/__init__.py` & `bagbag-0.60.0/src/bagbag/Funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Hash/__init__.py` & `bagbag-0.60.0/src/bagbag/Hash/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Hash/src.py` & `bagbag-0.60.0/src/bagbag/Hash/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Http/__init__.py` & `bagbag-0.60.0/src/bagbag/Http/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Http/src.py` & `bagbag-0.60.0/src/bagbag/Http/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from random_user_agent.params import OperatingSystem as useragent_operatingsystem 
 
 useragents = useragent_generator(
     software_names=[
         useragent_softwarename.CHROME.value,
         useragent_softwarename.CHROMIUM.value,
         useragent_softwarename.EDGE.value,
-        useragent_softwarename.FIREFOX.value,
-        useragent_softwarename.OPERA.value,
+        # useragent_softwarename.FIREFOX.value,
+        # useragent_softwarename.OPERA.value,
     ], 
     operating_systems=[
         useragent_operatingsystem.WINDOWS.value,
         useragent_operatingsystem.LINUX.value,
         useragent_operatingsystem.MAC.value,
         useragent_operatingsystem.MAC_OS_X.value,
         useragent_operatingsystem.MACOS.value,
```

### Comparing `bagbag-0.59.8/src/bagbag/Json/src.py` & `bagbag-0.60.0/src/bagbag/Json/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     :return: A string
     """
     return json.dumps(obj, indent=indent, ensure_ascii=ensure_ascii)
 
 def Loads(s:str|io.TextIOWrapper) -> list | dict:
     """
     The function Loads can load JSON or HTML data from 
-    1. a file 
+    1. a file (file path)
     2. a string
     3. a file object
     
     :param s: The parameter `s` can be either a string or a file object (`io.TextIOWrapper`). It
-    represents the JSON data that needs to be loaded
+    represents the JSON data or HTML data that needs to be loaded
     :type s: str|io.TextIOWrapper
     :return: The function `Loads` returns a list or a dictionary depending on the input provided. If the
     input is a file object of type `io.TextIOWrapper`, it reads the contents of the file and returns a
     dictionary or a list after parsing the JSON data. If the input is a string, it checks if the string
     starts with `[` or `{` and returns a dictionary or a list after
     """
     if type(s) == io.TextIOWrapper:
```

### Comparing `bagbag-0.59.8/src/bagbag/Lg.py` & `bagbag-0.60.0/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Math/src.py` & `bagbag-0.60.0/src/bagbag/Math/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Os/Path/__init__.py` & `bagbag-0.60.0/src/bagbag/Os/Path/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Os/Path/src.py` & `bagbag-0.60.0/src/bagbag/Os/Path/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Os/__init__.py` & `bagbag-0.60.0/src/bagbag/Os/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
         "Getcwd",
         "Unlink",
         "Move",
         "Copy",
         "GetLoginUserName",
         "Walk",
         "GetUID",
+        "Args"
     ],
     "Path": ["Path"]
 }
 
 if TYPE_CHECKING:
     from .src import (
         Exit,
@@ -33,14 +34,15 @@
         Getcwd,
         Unlink,
         Move,
         Copy,
         GetLoginUserName,
         Walk,
         GetUID,
+        Args
     )
     from . import Path
 else:
     sys.modules[__name__] = LazyImporter(
         __name__,
         globals()["__file__"],
         _import_structure,
```

### Comparing `bagbag-0.59.8/src/bagbag/Os/src.py` & `bagbag-0.60.0/src/bagbag/Os/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Process/src.py` & `bagbag-0.60.0/src/bagbag/Process/src.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import multiprocessing 
-from typing import Any
 
 ## print("load process")
 
-def Process(func, *args:Any, daemon:bool=True) -> multiprocessing.Process:
+def Process(func, *args, daemon:bool=True) -> multiprocessing.Process:
     """
     注意调用这个函数的时候要放到if __name__ == "__main__"里面, 否则可能会报错
     
     `Process` is a function that takes a function and its arguments, and returns a
     `multiprocessing.Process` object that runs the function in a separate process. 
     
     :param func: The function to be executed
```

### Comparing `bagbag-0.59.8/src/bagbag/Python/src.py` & `bagbag-0.60.0/src/bagbag/Python/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Random/src.py` & `bagbag-0.60.0/src/bagbag/Random/src.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-import random 
+
 from typing import Any
-import copy
+
 
 print("load random")
 
 def Int(min:int, max:int) -> int:
+    import random 
     return random.randint(min, max)
 
 def Choice(obj:list|str) -> Any:
+    import random 
     return random.choice(obj)
 
 def String(length:int=8, charset:str="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789") -> str:
+    import random 
     res = []
     while len(res) < length:
         res.append(random.choice(charset))
     
     return "".join(res)
 
 def Shuffle(li:list) -> list:
+    import random 
+    import copy
     l = copy.copy(li)
     random.shuffle(l)
     return l
 
 if __name__ == "__main__":
     print(Choice("doijwoefwe"))
     print(String(5))
```

### Comparing `bagbag-0.59.8/src/bagbag/Socket/TCP/src.py` & `bagbag-0.60.0/src/bagbag/Socket/TCP/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/String/src.py` & `bagbag-0.60.0/src/bagbag/String/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-
-
-
-
-
-
 ## print("load string")
 
 sentimentAnalyzer = None
 
 addrPattern = {
     "xmr":      "4[0-9AB][1-9A-HJ-NP-Za-km-z]{93}",
     "bech32":   "bc(0([ac-hj-np-z02-9]{39}|[ac-hj-np-z02-9]{59})|1[ac-hj-np-z02-9]{8,87})",
```

### Comparing `bagbag-0.59.8/src/bagbag/Time/__init__.py` & `bagbag-0.60.0/src/bagbag/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Time/src.py` & `bagbag-0.60.0/src/bagbag/Time/src.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-import time
-import datetime
-import tqdm
-from dateutil.parser import parse as dateparser
-from dateutil.parser import ParserError
-
-from ..String import String
-
 print("load time")
 
 def FormatDuration(seconds:int) -> str:
+    import time
+
     return time.strftime("%H:%M:%S", time.gmtime(seconds))
 
-Now = time.time 
+def Now() -> float:
+    import time
+
+    return time.time()
 
 def Sleep(num:int=0, title:str=None, bar:bool=None):
     """
     Sleep(num:int, bar:bool=None)
     
     The first argument is an integer, and the second argument is a boolean. The second argument is
     optional, and if it is not provided, it will be set to True if the first argument is greater than 5,
@@ -23,25 +20,30 @@
     
     :param num: The number of seconds to sleep
     :type num: int
     :param bar: If True, a progress bar will be displayed. If False, no progress bar will be displayed.
     If None, a progress bar will be displayed if the number of seconds is greater than 5
     :type bar: bool
     """
+
+    import time
+
     if num == 0:
         while True:
             time.sleep(333)
     else:
         if bar == None:
             if num > 5:
                 bar = True 
             else:
                 bar = False
 
         if bar:
+            import tqdm
+
             num = int(num)
             for _ in tqdm.tqdm(range(num), total=num, leave=False, desc=title):
                 time.sleep(1)
         else:
             time.sleep(num)
 
 def Strftime(timestamp:float|int, format:str="%Y-%m-%d %H:%M:%S") -> str:
@@ -50,18 +52,22 @@
     
     :param format: The format string to use
     :type format: str
     :param timestamp: The timestamp to format
     :type timestamp: float|int
     :return: A string
     """
+    import datetime
+
     dobj = datetime.datetime.fromtimestamp(timestamp)
     return dobj.strftime(format)
 
 def parseTimeago(timestring:str) -> int|None:
+    from ..String import String
+
     if timestring == "just now":
         return int(Now())
     
     res = String(timestring).RegexFind('([0-9]+)([smhdw])')
     # print(res)
     if len(res) != 0:
         sm = {
@@ -112,14 +118,19 @@
     :param format: The format of the timestring
     :type format: str
     :param timestring: The string to be converted to a timestamp
     :type timestring: str
     :return: The timestamp of the datetime object.
     """
 
+    from dateutil.parser import parse as dateparser
+    from dateutil.parser import ParserError
+    from ..String import String
+    import datetime
+
     if format:
         dtimestamp = datetime.datetime.strptime(timestring, format).timestamp()
     else:
         if len(String(timestring).RegexFind('([0-9]+)([smhdw])')) != 0:
             dtimestamp = parseTimeago(timestring)
             if not dtimestamp:
                 raise Exception(f"不能解析时间字符串: {timestring}")
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Argparser_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Argparser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py` & `bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py` & `bagbag-0.60.0/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/BlockChain/Tron/src.py` & `bagbag-0.60.0/src/bagbag/Tools/BlockChain/Tron/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/CSV.py` & `bagbag-0.60.0/src/bagbag/Tools/CSV.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,23 @@
             self.fd.flush()
 
     def Close(self):
         self.fd.close()
     
     def Flush(self):
         self.fd.flush()
+    
+    def __enter__(self):
+        return self 
+    
+    def __exit__(self, exc_type, exc_value, traceback):
+        try:
+            self.Close()
+        except:
+            pass
 
 if __name__ == "__main__":
     w = Writer("test.csv")
 
     w.SetHeaders("h1", "h2")
 
     w.Write({"h1": "v1", "h2": '"v2,kkk|'})
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Chan_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Chan_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.60.0/src/bagbag/Tools/ComputerVision.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from ..Thread import Thread
 from .. import Time
 from .Ratelimit_src import RateLimit
 from .. import Socket
 from ..String import String
 from .. import Lg
-from ..Base64 import src
+from .. import Base64
 from .. import Http
 from .. import Json
 from .. import Random
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 here = os.path.dirname(os.path.abspath(__file__))
@@ -260,15 +260,15 @@
         detections = netyolo.forward(output_layers)
 
         return cvStreamFrameObjectDetectionResult(detections, self.objectDetectModel, self.frame)
 
     def objectsByAPIServer(self) -> cvStreamFrameObjectDetectionResult:
         (flag, encodedImage) = cv2.imencode(".jpg", self.frame)
         encodedImage = bytearray(encodedImage)
-        encodedImage = src.Encode(encodedImage)
+        encodedImage = Base64.Encode(encodedImage)
 
         a = self.objectDetectModel.split("|")
         server = a[1]
         model = a[2]
 
         if not server.startswith("http://") and not server.startswith("https://"):
             server = "https://" + server
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Crontab_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Crontab_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from __future__ import annotations
 
 import schedule
 import time 
 
-try:
-    from ..Thread import Thread
-except:
-    import sys 
-    sys.path.append("..")
-    from Thread import Thread
+from ..Thread import Thread
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class Crontab():
     def __init__(self):
         Thread(self.run)
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/__init__.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/application.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/models/make_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/connection.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/connection_interface.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/mysql_connection.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/postgres_connection.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/connection_factory.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/connector.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/database_manager.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/column.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/column_diff.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/comparator.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/index.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/schema_manager.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/table.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/dbal/table_diff.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/events/__init__.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/connectors.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/exceptions/orm.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/migration_creator.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/migrator.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/migrations/stubs.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/builder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/collection.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/factory.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/factory_builder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/model.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_one.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/pivot.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/relation.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/result.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/orm/utils.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/base.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/pagination/paginator.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/builder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/join_clause.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/query/processors/processor.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/blueprint.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/builder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/mysql_builder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/schema/schema.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/seeds/seeder.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/fluent.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/support/grammar.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/__init__.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/command_formatter.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/helpers.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/qmarker.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/orator/utils/url.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Database/src.py` & `bagbag-0.60.0/src/bagbag/Tools/Database/src.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 from __future__ import annotations
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from . import orator
-    from ..Lock_src import Lock
-    from ... import Lg
-    from ... import Base64
-    from ... import Time 
-    from ..Redis_src import redisKey
-except:
-    import orator
-    from Lock_src import Lock
-    import sys
-    sys.path.append("...")
-    import Lg
-    import Base64
-    import Time 
+from . import orator
+from ..Lock_src import Lock
+from ... import Lg
+from ... import Base64
+from ... import Time 
+from ..Redis_src import redisKey
 
 import pickle
 import typing
 import bagbag
 import pymysql
 import threading
 import copy
@@ -160,15 +151,15 @@
     def avoidError(func): # func是被包装的函数
         def ware(self, *args, **kwargs): # self是类的实例
             if self.db.driver == "mysql":
                 while True:
                     try:
                         res = func(self, *args, **kwargs)
                         break
-                    except bagbag.Tools.orator.exceptions.query.QueryException as e:
+                    except orator.exceptions.query.QueryException as e:
                         if str(e).startswith('(1054, ') or str(e).startswith('(1406, '):
                             raise e 
                         # MySQL驱动默认不允许一个连接跨多个线程, 重连就行
                         Lg.Trace("重连, 因为:", e)
                         self.db.db.reconnect()
                     except pymysql.err.OperationalError as e:  
                         if e.args[0] == 2003:
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/DistributedLock_src.py` & `bagbag-0.60.0/src/bagbag/Tools/DistributedLock_src.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,18 @@
 #     environment:
 #       PASSWORD: password
 #       DEBUG: "False"
 
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from .. import Time
-    from .. import Http
-    from ..Thread import Thread
-    from .. import Lg
-except:
-    import sys
-    sys.path.append("..")
-    import Time
-    import Http
-    from Thread import Thread
-    import Lg
+from .. import Time
+from .. import Http
+from ..Thread import Thread
+from .. import Lg
 
 class distributedLockLock():
     def __init__(self, lockserver:DistributedLock, lockname:str, timeout:int) -> None:
         self.lockserver = lockserver
         self.lockname = lockname 
         self.timeout = timeout
         self.islocked = False
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Elasticsearch_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Elasticsearch_src.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import json 
 import time 
 import requests
 
-try:
-    from .. import Http, Lg
-except:
-    import sys 
-    sys.path.append("..")
-    import Http, Lg
+from .. import Http, Lg
 
 # requests.exceptions.ReadTimeout
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 def retryOnNetworkError(func): # func是被包装的函数
     def ware(self, *args, **kwargs): # self是类的实例
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/File_src.py` & `bagbag-0.60.0/src/bagbag/File/src.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
-import time
+
 import typing
-import magic
-import mimetypes
-from .. import Hash
 
-print("load file")
+# print("load file")
 
 class File():
     def __init__(self, path:str):
         self.path = path 
 
     def Md5Sum(self) -> str:
+        from .. import Hash
         return Hash.Md5sumFile(self.path)
 
     def AbsPath(self) -> str:
         return os.path.abspath(self.path)
 
     def Basename(self) -> str:
         return os.path.basename(self.path)
@@ -78,36 +76,40 @@
                 return 
     
     def TypeDescription(self) -> str:
         """
         根据文件内容生成描述
         Example: PDF document, version 1.2
         """
+
+        import magic
         if not os.path.exists(self.path) or not os.path.isfile(self.path):
             raise Exception("文件不存在:", self.path)
         
         return magic.from_file(self.path)
     
     def MimeType(self) -> str:
         """
         根据文件内容生存mime类型
         """
         if not os.path.exists(self.path) or not os.path.isfile(self.path):
             raise Exception("文件不存在:", self.path)
         
+        import magic
         mime = magic.Magic(mime=True)
         return mime.from_file(self.path)
     
     def GuessSuffix(self) -> str:
         """
         根据文件内容生成扩展名
         返回值包括前置"."
         例如: .jpg
         :return: The file extension of the file.
         """
+        import mimetypes
         return mimetypes.guess_extension(self.MimeType())
     
     def Tailf(self, fromBegin:bool=False, separator:str='\n', interval:int|float=1) -> typing.Iterable[str]:
         """
         It reads the file in chunks of 4096 bytes, and yields the lines as they are read.
         Waiting for new lines come when reach the end of the file.
         Will read from the beginning of the file if the file gets truncate.
@@ -115,14 +117,16 @@
         :param fromBegin: If True, the tail will start from the beginning of the file, defaults to False
         :type fromBegin: bool (optional)
         :param separator: The separator to use when splitting the file, defaults to \n
         :type separator: str (optional)
         :param interval: The time to wait between checking the file for new lines, defaults to 1 second
         :type interval: int|float (optional)
         """
+        import time
+        
         lfsize = self.Size()
 
         stream = open(self.path)
         if not fromBegin:
             stream.seek(0, os.SEEK_END)
 
         buffer = ''
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Github_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Github_src.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 from __future__ import annotations
 
 from github import Github as githubclient
 from github.GithubException import RateLimitExceededException
 from github.GithubException import GithubException
 
-try:
-    from .. import Http
-    from .Ratelimit_src import RateLimit
-    from ..String import String
-    from .. import Time
-    from .. import Lg
-except:
-    from Ratelimit_src import RateLimit
-    import sys
-    sys.path.append("..")
-    import Http
-    from String import String
-    import Time
-    import Lg
+from .. import Http
+from .Ratelimit_src import RateLimit
+from ..String import String
+from .. import Time
+from .. import Lg
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 import typing
 
 # class GithuException(Exception):
 #     pass
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/JavaScript_src.py` & `bagbag-0.60.0/src/bagbag/Tools/JavaScript_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Lock_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Lock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/MatrixBot_src.py` & `bagbag-0.60.0/src/bagbag/Tools/MatrixBot_src.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,26 +24,17 @@
 # 版本0.0.1
 #     arm64的可以调用http api发送消息, 也可以收消息(发送id给bot返回房间号)
 #     amd64的可以调用http api发送消息, 但是不能收消息, 一脸蒙逼
 #     
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from .. import Http
-    from ..Base64 import src
-    from .. import Json
-    from .. import Lg
-except:
-    import sys
-    sys.path.append("..")
-    import Http 
-    import Base64
-    import Lg
-    import Json
+from .. import Http
+from .. import Base64
+from .. import Json
 
 import requests
 import time
 
 def retryOnNetworkError(func): # func是被包装的函数
     def ware(self, *args, **kwargs): # self是类的实例
         while True:
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/OCR_src.py` & `bagbag-0.60.0/src/bagbag/Tools/OCR_src.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,24 +11,17 @@
 #     restart: always
 #     ports:
 #       - 8990:8990
 # 
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from .. import Http
-    from ..Base64 import src
-    from .. import Json
-except:
-    import sys 
-    sys.path.append("..")
-    import Http 
-    import Base64
-    import Json 
+from .. import Http
+from .. import Base64
+from .. import Json
 
 class ocrResultText():
     def __init__(self, Coordinate:list, Text:str, Confidence:float) -> None:
         self.Coordinate:list = Coordinate 
         self.Text:str = Text 
         self.Confidence:float = Confidence
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/ProgressBar_src.py` & `bagbag-0.60.0/src/bagbag/Tools/ProgressBar_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.60.0/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.60.0/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 
 import prometheus_client as pc
 import time
 import socket
 
 import threading
 
-from ...Base64 import src 
+from ... import Base64 
 
-try:
-    from .metrics import * 
-    from ... import Http, Tools, Lg
-except:
-    from metrics import * 
-    import sys 
-    sys.path.append("...")
-    import Http, Tools, Lg, Base64
+from .metrics import * 
+from ... import Http, Tools, Lg
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class PushGateway():
     def __init__(self, job:str, address:str, basicAuthUser:str=None, basicAuthPass:str=None, pushinterval:int=15, instance:str=None):
         self.job = job 
         self.instance = instance if instance != None else socket.gethostname()
@@ -57,14 +51,15 @@
             # print(self.address)
             if data != "":
                 while True:
                     try:
                         Http.PutRaw(self.address, data, headers=self.headers, timeoutRetryTimes=9999)
                         break 
                     except Exception as e:
+                        Lg.Warn(e)
                         time.sleep(1)
                         # print(e)
         
     def NewCounter(self, name:str, help:str) -> PrometheusCounter:
         return PrometheusCounter(name, help, self.registry)
     
     def NewCounterWithLabel(self, name:str, labels:list[str], help:str) -> PrometheusCounterVec:
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.60.0/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Queue_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Queue_src.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,17 @@
 #       # SQLITE_PATH: /data/queue.db
 
 #     # volumes:
 #     #   - /data/cr-volumes/queue-server/data:/data
     
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from .. import Http
-    from ..Base64 import src
-    from .. import Lg
-except:
-    import sys
-    sys.path.append("..")
-    import Http
-    import Base64
-    import Lg
+from .. import Http
+from .. import Base64
+from .. import Lg
 
 import typing
 import pickle
 
 class queueQueueConfirm():
     def __init__(self, server:str, name:str, length:int=0, timeout:int=300) -> None:
         self.server = server
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/RSS/Feed.py` & `bagbag-0.60.0/src/bagbag/Tools/RSS/Feed.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/RSS/Opml.py` & `bagbag-0.60.0/src/bagbag/Tools/RSS/Opml.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Ratelimit_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Ratelimit_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Redis_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Redis_src.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,17 @@
 import pickle
 import typing
 import time
 import shortuuid
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-try:
-    from .. import Lg
-    from ..Base64 import src
-    from ..Process import Process
-except:
-    import sys
-    sys.path.append("..")
-    import Lg
-    import Base64
-    from Process import Process
+from .. import Lg
+from .. import Base64
+from ..Process import Process
 
 class RedisException(Exception):
     pass 
 
 class RedisQueueClosed(RedisException):
     pass
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/SSH_src.py` & `bagbag-0.60.0/src/bagbag/Tools/SSH_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Selenium.py` & `bagbag-0.60.0/src/bagbag/Tools/Selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from ..Http import useragents 
 from .. import Lg
 from ..Thread import Thread
 from .URL_src import URL
 from ..String import String 
 from .. import Os
-from .File_src import File
+from ..File import File
 
 seleniumChromeWireSkipFilesSuffix = (
     # 图片
     '.png', 
     '.jpg', 
     '.gif', 
     '.jpeg', 
@@ -84,20 +84,20 @@
                 try:
                     res = func(self, *args, **kwargs)
 
                     try:
                         NeedRefresh = False
                         # 如果载入页面失败, 有个Reload的按钮
                         if hasattr(self, "Find"):
-                            if self.Find("/html/body/div[1]/div[2]/div/button[1]", 0):
-                                if self.Find("/html/body/div[1]/div[2]/div/button[1]").Text() == "Reload":
+                            if self._find("/html/body/div[1]/div[2]/div/button[1]", 0):
+                                if self._find("/html/body/div[1]/div[2]/div/button[1]").Text() == "Reload":
                                     NeedRefresh = True
                         elif hasattr(self, "se") and hasattr(self.se, "Find"):
-                            if self.se.Find("/html/body/div[1]/div[2]/div/button[1]", 0):
-                                if self.se.Find("/html/body/div[1]/div[2]/div/button[1]").Text() == "Reload":
+                            if self.se._find("/html/body/div[1]/div[2]/div/button[1]", 0):
+                                if self.se._find("/html/body/div[1]/div[2]/div/button[1]").Text() == "Reload":
                                     NeedRefresh = True
 
                         if hasattr(self, "PageSource"):
                             page = self.PageSource()
                         elif hasattr(self, "se") and hasattr(self.se, "PageSource"):
                             page = self.se.PageSource()
                         
@@ -267,15 +267,46 @@
         self.driver.execute_script("arguments[0].scrollIntoView(true);", self.element)
         return self
 
     def HTML(self) -> str:
         return self.element.get_attribute('innerHTML')
 
 class seleniumBase():
-    def Find(self, xpath:str, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> seleniumElement|None:
+    def Find(self, xpath:str|list, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> seleniumElement|None:
+        """
+        This is a Python function that finds a Selenium element based on an XPath string or list of XPath
+        strings, with optional parameters for timeout, scrolling, and retrying on errors.
+        
+        :param xpath: The xpath expression used to locate the element(s) on the webpage
+        :type xpath: str|list
+        :param timeout: The maximum amount of time (in seconds) to wait for the element to be found before
+        timing out and returning None, defaults to 60
+        :type timeout: int (optional)
+        :param scrollIntoElement: scrollIntoElement is a boolean parameter that determines whether the web
+        page should be scrolled to bring the element into view before attempting to find it using the
+        specified XPath. If set to True, the page will be scrolled to bring the element into view before
+        attempting to find it. If set to False, the, defaults to True
+        :type scrollIntoElement: bool (optional)
+        :param retryOnError: The retryOnError parameter specifies the number of times the function should
+        retry finding the element if an error occurs during the search. If the element is not found after
+        the specified number of retries, the function will return None, defaults to 5
+        :type retryOnError: int (optional)
+        :return: The function `Find` returns a `seleniumElement` object if it is found, or `None` if it is
+        not found.
+        """
+        if type(xpath) == str:
+            return self._find(xpath, timeout, scrollIntoElement, retryOnError)
+        else:
+            idx = self.Except(xpath, timeout=timeout)
+            if idx == None:
+                return None 
+            else:
+                return self._find(xpath[idx], timeout, scrollIntoElement, retryOnError)
+
+    def _find(self, xpath:str, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> seleniumElement|None:
         """
         > Finds an element by xpath, waits for it to appear, and returns it
         
         :param xpath: The xpath of the element you want to find
         :type xpath: str
         :param timeout: , defaults to 8 second
         :type timeout: int (optional)
@@ -311,15 +342,15 @@
                 else:
                     raise e 
 
         # import ipdb
         # ipdb.set_trace()
     
     def Exists(self, xpath:str, timeout:int=0) -> bool:
-        return self.Find(xpath, timeout=timeout) != None
+        return self._find(xpath, timeout=timeout) != None
     
     def StatusCode(self) -> int:
         self.driver.stat
     
     def ResizeWindow(self, width:int, height:int):
         """
         :param width: The width of the window in pixels
@@ -467,30 +498,30 @@
             try:
                 self.driver.execute_script("const dbs = await window.indexedDB.databases();dbs.forEach(db => { window.indexedDB.deleteDatabase(db.name)});")
             except:
                 pass
         else:
             raise Exception("未实现")
     
-    def Except(self, *xpath:str, timeout:int=30) -> int | None:
+    def Except(self, *xpath:str|list, timeout:int=30) -> int | None:
         """
         It waits for some certain elements to appear on the screen.
         
         :param : xpath:str - The xpaths of the element you want to find
         :type : str
         :param timeout: The number of seconds to wait for the element to appear, defaults to 30
         :type timeout: int (optional)
         :return: The index of the xpath that is found.
         """
         if type(xpath[0]) == list:
             xpath = xpath[0]
             
         for _ in range(timeout*2):
             for x in range(len(xpath)):
-                if self.Find(xpath[x], 0, scrollIntoElement=False):
+                if self._find(xpath[x], 0, scrollIntoElement=False):
                     return x
             time.sleep(0.5)
 
         return None 
     
     def SwitchTabByID(self, number:int):
         """
@@ -557,14 +588,16 @@
             )
         else:
             self.driver = webdriver.Firefox(options=options)
         
         if sessionID:
             self.Close()
             self.driver.session_id = sessionID
+        
+        self.ResizeWindow(1400, 1400)
 
         self.browserName = "firefox"
         self.browserRemote = seleniumServer != None 
 
 class Chrome(seleniumBase):
     def __init__(
             self, 
@@ -613,14 +646,16 @@
                 options=options,
             )
 
         if sessionID:
             self.Close()
             self.driver.session_id = sessionID
         
+        self.ResizeWindow(1400, 1400)
+        
         self.browserName = "chrome"
         self.browserRemote = seleniumServer != None 
         self.closed = False
 
 class seleniumFlowRequest():
     def __init__(self) -> None:
         self.Time:int = None 
@@ -756,14 +791,16 @@
         if blockSuffix != None:
             self.driver.request_interceptor = interceptor
 
         if sessionID:
             self.Close()
             self.driver.session_id = sessionID
         
+        self.ResizeWindow(1400, 1400)
+        
         self.browserName = "chromewire"
         self.browserRemote = False
         self.closed = False
         self.blockSuffix = blockSuffix
     
     def Flows(self, clean:bool=True) -> typing.Iterable[seleniumFlow]:
         """
@@ -797,15 +834,20 @@
                 fresp = seleniumFlowResponse()
                 fresp.Headers = {}
                 for key in resp.headers:
                     fresp.Headers[key] = resp.headers[key]
                 fresp.StatusCode = resp.status_code
                 fresp.Time = resp.date.timestamp()
                 if resp.body != None:
-                    fresp.BodyBytes = decodeResponseBody(resp.body, resp.headers.get('Content-Encoding', 'identity'))
+                    try:
+                        fresp.BodyBytes = decodeResponseBody(resp.body, resp.headers.get('Content-Encoding', 'identity'))
+                    except Exception as e:
+                        Lg.Warn("解码body报错:", e)
+                        fresp.BodyBytes = b''
+
                     fresp.Body = fresp.BodyBytes.decode(errors="ignore")
                     # if 'content-encoding' not in fresp.Headers:
                     #     fresp.Body = resp.body.decode(errors="ignore")
                     #     fresp.BodyBytes = resp.body 
                     # else:
                     #     if fresp.Headers['content-encoding'].strip() == 'br':
                     #         # Lg.Trace("Before:", resp.body[:80])
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.60.0/src/bagbag/Tools/TelegramAsync.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/TelegramBotOfficial_src.py` & `bagbag-0.60.0/src/bagbag/Tools/TelegramBotOfficial_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/TelegramBot_src.py` & `bagbag-0.60.0/src/bagbag/Tools/TelegramBot_src.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 from __future__ import annotations
 
-try:
-    from .. import Http
-    from .. import Time
-    from .. import Lg
-    from ..Base64 import src
-    from ..File_src import File
-    from .. import Funcs
-except:
-    import sys
-    sys.path.append("..")
-
-    import Http
-    import Time
-    import Lg
-    import Base64
-    from File_src import File
-    import Funcs
+from .. import Http
+from .. import Time
+from .. import Lg
+from .. import Base64 
+from . import File
+from .. import Funcs
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 import msgpack
 import os
 
 # 配合这个镜像使用
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Telegram_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Telegram_src.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,34 +18,22 @@
 from telethon.tl.types import  InputMessagesFilterVoice
 import tqdm
 
 from hachoir.metadata import extractMetadata
 from hachoir.parser import createParser
 from telethon.tl.types import DocumentAttributeVideo
 
-try:
-    from .. import Os
-    from .Database_src import SQLite
-    from .. import Time
-    from .. import Lg
-    from ..String import String
-    from .File_src import File
-    from .Ratelimit_src import RateLimit
-    from .. import Funcs
-except:
-    import sys 
-    sys.path.append("..")
-    import Os
-    from Database_src import SQLite
-    import Time
-    import Lg
-    from String import String
-    from File_src import File
-    from Ratelimit_src import RateLimit
-    import Funcs
+from .. import Os
+from .Database import SQLite
+from .. import Time
+from .. import Lg
+from ..String import String
+from ..File import File
+from .Ratelimit_src import RateLimit
+from .. import Funcs
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class TelegramGeo():
     def __init__(self):
         self.Long = None
         self.Lat = None
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Translater_src.py` & `bagbag-0.60.0/src/bagbag/Tools/Translater_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Twitter/Elevated.py` & `bagbag-0.60.0/src/bagbag/Tools/Twitter/Elevated_src.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import tweepy
 import typing 
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
 class twitterUser():
     def __init__(self) -> None:
@@ -33,35 +34,59 @@
     
     def __repr__(self) -> str:
         return f"twitterUserMention(ID={self.ID} ScreenName={self.ScreenName} Name={self.Name})"
     
     def __str__(self) -> str:
         return self.__repr__()
 
-class twitterTweet():
+class ElevatedTweet():
     def __init__(self) -> None:
         self.ID:int = None
         self.User:twitterUser = None 
         self.Time:int = None 
         self.Text:str = None 
         self.Language:str = None 
         self.FavoriteCount:int = None 
         self.RetweetCount:int = None 
         self.Mentions:list[twitterUserMention] = []
         self.Urls:list[str] = []
         self.Media:list[str] = []
         self.Tag:list[str] = []
-        self.raw_data:dict = None 
-    
+        self.WebURL:str = None 
+
+        self.raw_data:dict = None
+        
+        self.in_reply_to_tweet_id:int = None
+        self.twitter:Elevated = None 
+
     def __repr__(self) -> str:
-        return f"twitterTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text} User={self.User} FavoriteCount={self.FavoriteCount} RetweetCount={self.RetweetCount} UserMentions={self.UserMentions} Urls={self.Urls} Media={self.Media} Tags={self.Tags})"
+        return f"ElevatedTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text} User={self.User} FavoriteCount={self.FavoriteCount} RetweetCount={self.RetweetCount} Mentions={self.Mentions} Urls={self.Urls} Media={self.Media} Tag={self.Tag} WebURL={self.WebURL})"
     
     def __str__(self) -> str:
         return self.__repr__()
 
+    def InReplyToTweet(self) -> ElevatedTweet | None:
+        if self.in_reply_to_tweet_id == None:
+            return None 
+        
+        return self.twitter.Tweet(self.in_reply_to_tweet_id)
+
+    def Replies(self) -> list[ElevatedTweet]:
+        res = []
+        # print(75, "to:" + self.User.ScreenName)
+        for t in self.twitter.Search("to:" + self.User.ScreenName):
+            # print(77, t)
+            # print(t.in_reply_to_status_id, self.ID)
+            # print(type(t.in_reply_to_status_id), type(self.ID))
+            if t.in_reply_to_tweet_id == self.ID:
+                res.append(t)
+            # print('')
+
+        return res
+
 class Elevated():
     def __init__(self, consumer_key:str, consumer_secret:str) -> None:
         auth = tweepy.OAuth2AppHandler(consumer_key, consumer_secret)
 
         self.api = tweepy.API(auth, wait_on_rate_limit=True)
     
     def _wrapUser(self, user) -> twitterUser:
@@ -76,26 +101,32 @@
         u.FollowersCount = user.followers_count
         u.StatusesCount = user.statuses_count
         u.Verified = user.verified
         u.raw_data = user._json
 
         return u
     
-    def _wrapStatus(self, status) -> twitterTweet:
+    def _wrapStatus(self, status) -> ElevatedTweet:
+        # import ipdb
+        # ipdb.set_trace()
         u = self._wrapUser(status.author)
 
-        t = twitterTweet()
+        t = ElevatedTweet()
+        t.twitter = self
         t.User = u 
 
         t.ID = status.id # https://twitter.com/saepudin1991/status/1613434061741260803
         t.Time = int(status.created_at.timestamp())
         t.FavoriteCount = status.favorite_count
         t.RetweetCount = status.retweet_count
         t.raw_data = status._json
 
+        if hasattr(status, 'in_reply_to_status_id_str'):
+            t.in_reply_to_tweet_id = status.in_reply_to_status_id
+
         if hasattr(status, 'retweeted_status'):
             # 由于如果是转推, 那么status.full_text会被截断到140个字符, 而完整的推文在status.retweeted_status.full_text
             # 所以拼接一下
             sidx = 0
             foundsidx = False 
             while True:
                 if sidx > 140 or status.full_text[sidx:-1] == "":
@@ -135,18 +166,20 @@
             if 'media' in status.entities and len(status.entities['media']) != 0:
                 for u in status.entities['media']:
                     t.Media.append(u['media_url'])
 
             if 'hashtags' in status.entities and len(status.entities['hashtags']) != 0:
                 for u in status.entities['hashtags']:
                     t.Tag.append(u['text'])
+        
+        t.WebURL = f"https://twitter.com/{t.User.ScreenName}/status/{t.ID}"
 
         return t
     
-    def Search(self, keyword:str, includeReTweets:bool=False, days:int=7, countPerRequest:int=40, sinceID:int=None) -> typing.Iterable[twitterTweet]:
+    def Search(self, keyword:str, includeReTweets:bool=False, days:int=7, countPerRequest:int=40, sinceID:int=None) -> typing.Iterable[ElevatedTweet]:
         """
         It takes a keyword, and returns an iterator of tweets that contain that keyword. 
         tweet的ID是从大到小, 也就是数据的时间是从近到远
         
         :param keyword: The keyword to search for
         :type keyword: str
         :param days: How many days back to search, defaults to 7
@@ -162,15 +195,15 @@
             keyword = keyword + " -filter:retweets"
             
         for status in tweepy.Cursor(self.api.search_tweets, q=keyword, tweet_mode='extended', count=countPerRequest, since_id=sinceID).items():
             # import ipdb
             # ipdb.set_trace()
             yield self._wrapStatus(status)
     
-    def Timeline(self, screenameOrID:str|int, countPerRequest:int=40, sinceID:int=None, includeReTweets:bool=False) -> typing.Iterable[twitterTweet]:
+    def Timeline(self, screenameOrID:str|int, countPerRequest:int=40, sinceID:int=None, includeReTweets:bool=False) -> typing.Iterable[ElevatedTweet]:
         """
         tweet from the timeline of the user with the given screen name
         tweet的ID是从大到小, 也就是数据的时间是从近到远
         如果有sinceID, 就返回比这个sinceID更新的tweets, 不包括这个tweet
         
         :param screename: The screen name of the user
         :type screename: str
@@ -205,21 +238,21 @@
             user = self.api.get_user(screen_name=screenameOrID)
         elif type(screenameOrID) == int:
             user = self.api.get_user(user_id=screenameOrID)
         # import ipdb
         # ipdb.set_trace()
         return self._wrapUser(user)
 
-    def Tweet(self, tid:int) -> twitterTweet:
+    def Tweet(self, tid:int) -> ElevatedTweet:
         return self._wrapStatus(self.api.get_status(tid, tweet_mode = "extended"))
 
 if __name__ == "__main__":
-    import json 
+    from bagbag import Lg, Json
 
-    cfg = json.loads(open('twitter.ident').read())
+    cfg = Json.Loads(open('twitter.ident').read())
 
     twitter = Elevated(cfg['consumer_key'], cfg['consumer_secret'])
 
     # print("user")
     # u = twitter.User("asiwaju_wa")
     # print(u)
     
@@ -237,9 +270,15 @@
     #         break 
     
     # print("followers")
     # for i in twitter.Followers("asiwaju_wa"):
     #     print(i)
     #     break 
 
-    import ipdb
-    ipdb.set_trace()
+    t = twitter.Tweet(1660223526509625349)
+    Lg.Trace(t)
+
+    ts = t.Replies()
+    Lg.Trace(ts)
+
+    # import ipdb
+    # ipdb.set_trace()
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Twitter/Essential.py` & `bagbag-0.60.0/src/bagbag/Tools/Twitter/Essential_src.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import tweepy
 import typing 
 
 tweetFields = ['author_id', 'created_at', 'geo', 'id', 'lang', 'text']
 
 print("load " + '/'.join(__file__.split('/')[-2:]))
 
-class twitterTweet():
+class EssentialTweet():
     def __init__(self) -> None:
         self.ID:int = None
         self.Time:int = None 
         self.Text:str = None 
         self.Language:str = None 
     
     def __repr__(self) -> str:
-        return f"twitterTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text})"
+        return f"EssentialTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text})"
     
     def __str__(self) -> str:
-        return f"twitterTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text})"
+        return f"EssentialTweet(ID={self.ID} Time={self.Time} Language={self.Language} Text={self.Text})"
 
 class Essential():
     def __init__(self, bearerToken:str) -> None:
         self.api = tweepy.Client(bearer_token=bearerToken, wait_on_rate_limit=True)
 
-    def _wrapStatus(self, status) -> twitterTweet:
-        t = twitterTweet()
+    def _wrapStatus(self, status) -> EssentialTweet:
+        t = EssentialTweet()
 
         t.ID = status.id 
         t.Time = int(status.created_at.timestamp())
 
         t.Text = status.text
 
         t.Language = status.lang
 
         return t
     
-    def Search(self, keyword:str, sinceID:int=None, tweetPerRequest:int=10) -> typing.Iterable[twitterTweet]:
+    def Search(self, keyword:str, sinceID:int=None, tweetPerRequest:int=10) -> typing.Iterable[EssentialTweet]:
         tweets = tweepy.Paginator(self.api.search_recent_tweets, query=keyword, since_id=sinceID, tweet_fields=tweetFields, max_results=tweetPerRequest).flatten()
         for status in tweets:
             yield self._wrapStatus(status)
     
-    def Timeline(self, screename:str, sinceID:int=None, tweetPerRequest:int=10) -> typing.Iterable[twitterTweet]:
+    def Timeline(self, screename:str, sinceID:int=None, tweetPerRequest:int=10) -> typing.Iterable[EssentialTweet]:
         u = self.api.get_user(username=screename)
         if len(u.errors) != 0:
             raise Exception("User not exists: " + screename)
 
         tweets = tweepy.Paginator(self.api.get_users_tweets, id=u.data.id, since_id=sinceID, tweet_fields=tweetFields, max_results=tweetPerRequest).flatten()
         for status in tweets:
             yield self._wrapStatus(status)
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/URL_src.py` & `bagbag-0.60.0/src/bagbag/Tools/URL_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/WaitGroup_src.py` & `bagbag-0.60.0/src/bagbag/Tools/WaitGroup_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/WebCrawler_src.py` & `bagbag-0.60.0/src/bagbag/Tools/WebCrawler_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/WebServer_src.py` & `bagbag-0.60.0/src/bagbag/Tools/WebServer_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/XPath_src.py` & `bagbag-0.60.0/src/bagbag/Tools/XPath_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.59.8/src/bagbag/Tools/Xlsx.py` & `bagbag-0.60.0/src/bagbag/Tools/Xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,17 @@
     
     def __exit__(self, exc_type, exc_value, traceback):
         try:
             self.Close()
         except:
             pass
 
-class Xlsx:
-    Reader
-    Writer
+# class Xlsx:
+#     Reader
+#     Writer
 
 if __name__ == "__main__":
     w = Writer("test.xlsx")
 
     w.SetHeaders("h1", "h2")
 
     w.Write({"h1": "v1", "h2": '"v2,kkk|'})
```

### Comparing `bagbag-0.59.8/src/bagbag/Tools/__init__.py` & `bagbag-0.60.0/src/bagbag/Tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,52 +44,54 @@
     # from . import BlockChain
     "BlockChain": ["BlockChain"], 
     "JavaScript": ["JavaScript"],
     # from . import ComputerVision
     "ComputerVision": ["ComputerVision"],
     "WebCrawler_src": ["WebCrawler"],
     "OCR_src": ["OCR"],
-    "File_src": ["File"],
+    # "File_src": ["File"],
     "Selenium": ["Selenium"],
     "CSV": ["CSV"],
     "Prometheus": ['Prometheus'],
+    "Cache": ["Cache"]
 }
 
 if TYPE_CHECKING:
-    from .File_src import File
+    # from ..File_src import File
     from .Redis_src import Redis, redisQueue, redisQueueConfirm
     from .Database import SQLite, MySQL, mySQLSQLiteKeyValueTable, mySQLSQLiteTable,mySQLSQLiteQueue, mySQLSQLiteConfirmQueue
     from .ProgressBar_src import ProgressBar
     from .Telegram_src import Telegram, TelegramPeer
+    from . import Cache
     from . import CSV
     from . import Selenium
     from .Lock_src import Lock
     from . import Prometheus
     from .URL_src import URL
     from .Ratelimit_src import RateLimit
     from .Chan_src import Chan
     from .WebServer_src import WebServer
     from .TelegramBotOfficial_src import TelegramBotOfficial
     from .TelegramBot_src import TelegramBot
     from .Argparser_src import Argparser
     from .Elasticsearch_src import Elasticsearch
     from .Crontab_src import Crontab
     from .WaitGroup_src import WaitGroup
-    from .Xlsx import Xlsx
+    from . import Xlsx
     from .XPath_src import XPath
     from .Translater_src import Translater
     from .SSH_src import SSH
     # from .TelegramAsync import TelegramAsync
     from .Github_src import Github
     from .Kafka_src import Kafka, kafkaProducer, kafkaConsumer
     from .Queue_src import Queue
     from .RSS import RSS
     from .MatrixBot_src import MatrixBot
     from .Nslookup_src import Nslookup
-    from .Twitter import Twitter
+    from . import Twitter
     from .DistributedLock_src import DistributedLock
     # from .Test import Test
     from .BlockChain import BlockChain
     from .JavaScript_src import JavaScript
     from .ComputerVision import ComputerVision
     from .WebCrawler_src import WebCrawler
     from .OCR_src import OCR
```

### Comparing `bagbag-0.59.8/src/bagbag/__init__.py` & `bagbag-0.60.0/src/bagbag/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-
-
 from . import Lg # 不能lazyimport,会功能有问题
 
 # def Size(ByteNumber, suffix='B'):
 #     for unit in ['','K','M','G','T','P','E','Z']:
 #         if abs(ByteNumber) < 1024.0:
 #             return "%3.1f%s%s" % (ByteNumber, unit, suffix)
 #         ByteNumber /= 1024.0
@@ -45,14 +43,16 @@
 # Lg.Trace(Size(process.memory_info().rss))
 
 from . import Funcs
 # Lg.Trace(Size(process.memory_info().rss))
 from . import Tools
 # Lg.Trace(Size(process.memory_info().rss))
 
+from .File import File
+
 # 
 # 如果导入包是from bagbag import * 则lazyimport无效, 如果是import bagbag 就有效
 # 
 # from typing import TYPE_CHECKING
 # from lazy_imports import LazyImporter
 # import sys
 # _import_structure = {
@@ -78,14 +78,15 @@
 # Lg.Trace(Size(process.memory_info().rss))
 from .Process import Process
 # Lg.Trace(Size(process.memory_info().rss))
 from .Python import Range
 # Lg.Trace(Size(process.memory_info().rss))
 from .String import String
 # Lg.Trace(Size(process.memory_info().rss))
+from .File import File
 
 if None not in [Os.Getenv("MATRIX_API_HOST"), Os.Getenv("MATRIX_API_PASS"), Os.Getenv("MATRIX_API_ROOM")]:
     def vWR0AQ68tikimG50():
         cwd = Os.Getcwd()
         stime = Time.Now()
         Time.Sleep(300, bar=False)
 
@@ -127,14 +128,16 @@
 
         mb = Tools.MatrixBot(Os.Getenv("MATRIX_API_HOST"), Os.Getenv("MATRIX_API_PASS")).SetRoom(Os.Getenv("MATRIX_API_ROOM"))
         # fname = Os.Path.Basename(sys.argv[0])
         
         # mb.Send(Time.Strftime(stime) + "\n" + msg + "\nStarted: " + fname)
 
         def sendwhenexit(stime:float, mb:Tools.MatrixBot):
+            Lg.Trace(traceback.format_exc())
+
             etime = Time.Now()
 
             while True:
                 try:
                     mb.Send(Time.Strftime(etime) + "\n" + msg + "\n\nExit\n\nDir: " + cwd + "\nCmd: " + ' '.join(sys.argv) + "\nDur: " + Funcs.Format.TimeDuration(etime - stime))
                     break
                 except Exception as e:
```

### Comparing `bagbag-0.59.8/PKG-INFO` & `bagbag-0.60.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.59.8
+Version: 0.60.0
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,15 @@
 Requires-Dist: Pillow (>=9.2.0)
 Requires-Dist: PyGithub (>=1.57)
 Requires-Dist: PyMySQL (>=1.0.2)
 Requires-Dist: Pygments (>=2.2)
 Requires-Dist: backpack (>=0.1)
 Requires-Dist: beautifulsoup4 (>=4.11.1)
 Requires-Dist: blinker (>=1.4)
+Requires-Dist: cachetools (>=4.2.4)
 Requires-Dist: cleo (>=0.6)
 Requires-Dist: feedparser (>=6.0.10)
 Requires-Dist: hachoir (>=3.2.0)
 Requires-Dist: html-to-json (>=2.0.0)
 Requires-Dist: inflection (>=0.3)
 Requires-Dist: ipdb (>=0.13.9)
 Requires-Dist: jieba (>=0.42.1)
```

