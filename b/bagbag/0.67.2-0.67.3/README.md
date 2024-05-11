# Comparing `tmp/bagbag-0.67.2.tar.gz` & `tmp/bagbag-0.67.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagbag-0.67.2.tar", max compression
+gzip compressed data, was "bagbag-0.67.3.tar", max compression
```

## Comparing `bagbag-0.67.2.tar` & `bagbag-0.67.3.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.67.2/LICENSE
--rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.67.2/README.md
--rw-r--r--   0        0        0     2416 2024-05-10 12:51:35.320164 bagbag-0.67.2/pyproject.toml
--rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.67.2/src/bagbag/Base64/__init__.py
--rw-r--r--   0        0        0      480 2023-09-22 09:26:09.030151 bagbag-0.67.2/src/bagbag/Base64/src.py
--rw-r--r--   0        0        0      561 2023-08-29 18:20:15.861931 bagbag-0.67.2/src/bagbag/Cmd/__init__.py
--rw-r--r--   0        0        0     5946 2024-01-08 10:23:15.811164 bagbag-0.67.2/src/bagbag/Cmd/src.py
--rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.67.2/src/bagbag/Cryptoo/__init__.py
--rw-r--r--   0        0        0     2539 2023-09-22 09:26:44.572415 bagbag-0.67.2/src/bagbag/Cryptoo/src.py
--rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.67.2/src/bagbag/File/__init__.py
--rw-r--r--   0        0        0     5162 2023-08-18 05:52:04.823383 bagbag-0.67.2/src/bagbag/File/src.py
--rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.67.2/src/bagbag/Funcs/CutSentenceStopWords_src.py
--rw-r--r--   0        0        0      858 2023-09-22 09:26:44.571988 bagbag-0.67.2/src/bagbag/Funcs/CutSentence_src.py
--rw-r--r--   0        0        0     6833 2023-09-22 09:26:44.572042 bagbag-0.67.2/src/bagbag/Funcs/FakeIdentity_src.py
--rw-r--r--   0        0        0      558 2023-09-22 09:26:44.571998 bagbag-0.67.2/src/bagbag/Funcs/FileType_src.py
--rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.67.2/src/bagbag/Funcs/Format/__init__.py
--rw-r--r--   0        0        0      837 2023-09-22 09:26:44.572060 bagbag-0.67.2/src/bagbag/Funcs/Format/src.py
--rw-r--r--   0        0        0      753 2023-09-22 09:26:44.571981 bagbag-0.67.2/src/bagbag/Funcs/GetPublicIP_src.py
--rw-r--r--   0        0        0      296 2023-09-22 09:26:44.572371 bagbag-0.67.2/src/bagbag/Funcs/IPAddressConvert_src.py
--rw-r--r--   0        0        0      474 2023-09-22 09:26:44.572073 bagbag-0.67.2/src/bagbag/Funcs/Markdown_src.py
--rw-r--r--   0        0        0      996 2023-09-22 09:26:44.571956 bagbag-0.67.2/src/bagbag/Funcs/Ping_src.py
--rw-r--r--   0        0        0     1730 2023-09-22 09:26:44.571972 bagbag-0.67.2/src/bagbag/Funcs/ResizeImage_src.py
--rw-r--r--   0        0        0      181 2023-11-01 18:01:37.175603 bagbag-0.67.2/src/bagbag/Funcs/UUID_src.py
--rw-r--r--   0        0        0      511 2024-01-10 05:42:03.100032 bagbag-0.67.2/src/bagbag/Funcs/VersionCompare_src.py
--rw-r--r--   0        0        0     1458 2023-09-22 09:26:44.572132 bagbag-0.67.2/src/bagbag/Funcs/Wget_src.py
--rw-r--r--   0        0        0      219 2024-05-09 06:52:12.594416 bagbag-0.67.2/src/bagbag/Funcs/Whois_src.py
--rw-r--r--   0        0        0     1336 2024-05-09 06:40:19.129474 bagbag-0.67.2/src/bagbag/Funcs/__init__.py
--rw-r--r--   0        0        0     5364 2024-05-09 06:35:52.807587 bagbag-0.67.2/src/bagbag/Funcs/whois/__init__.py
--rw-r--r--   0        0        0   232589 2024-05-09 06:35:52.808013 bagbag-0.67.2/src/bagbag/Funcs/whois/data/public_suffix_list.dat
--rw-r--r--   0        0        0   127805 2024-05-09 06:53:24.503036 bagbag-0.67.2/src/bagbag/Funcs/whois/parser.py
--rw-r--r--   0        0        0     1518 2024-05-09 06:35:52.808434 bagbag-0.67.2/src/bagbag/Funcs/whois/time_zones.py
--rw-r--r--   0        0        0    15439 2024-05-09 06:35:52.808590 bagbag-0.67.2/src/bagbag/Funcs/whois/whois.py
--rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.67.2/src/bagbag/Hash/__init__.py
--rw-r--r--   0        0        0     1451 2023-09-22 09:26:44.572298 bagbag-0.67.2/src/bagbag/Hash/src.py
--rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.67.2/src/bagbag/Http/__init__.py
--rw-r--r--   0        0        0    12346 2023-09-22 09:26:44.571920 bagbag-0.67.2/src/bagbag/Http/src.py
--rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.67.2/src/bagbag/Json/__init__.py
--rw-r--r--   0        0        0     3272 2023-09-22 09:26:44.572028 bagbag-0.67.2/src/bagbag/Json/src.py
--rw-r--r--   0        0        0    10860 2023-06-16 14:21:52.035937 bagbag-0.67.2/src/bagbag/Lg.py
--rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.67.2/src/bagbag/Math/__init__.py
--rw-r--r--   0        0        0     2076 2023-09-22 09:26:44.572144 bagbag-0.67.2/src/bagbag/Math/src.py
--rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.67.2/src/bagbag/Os/Path/__init__.py
--rw-r--r--   0        0        0     1889 2023-09-22 09:26:44.571833 bagbag-0.67.2/src/bagbag/Os/Path/src.py
--rw-r--r--   0        0        0     1047 2023-09-29 15:45:37.749849 bagbag-0.67.2/src/bagbag/Os/__init__.py
--rw-r--r--   0        0        0     3468 2023-09-29 15:42:54.859953 bagbag-0.67.2/src/bagbag/Os/src.py
--rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.67.2/src/bagbag/Process/__init__.py
--rw-r--r--   0        0        0     1239 2023-06-15 09:27:23.720590 bagbag-0.67.2/src/bagbag/Process/src.py
--rw-r--r--   0        0        0      447 2023-10-18 11:52:42.930164 bagbag-0.67.2/src/bagbag/Python/__init__.py
--rw-r--r--   0        0        0     1650 2023-11-05 14:21:13.197206 bagbag-0.67.2/src/bagbag/Python/src.py
--rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.67.2/src/bagbag/Random/__init__.py
--rw-r--r--   0        0        0      817 2024-01-12 08:21:43.555903 bagbag-0.67.2/src/bagbag/Random/src.py
--rw-r--r--   0        0        0      510 2023-07-19 13:13:12.245619 bagbag-0.67.2/src/bagbag/Socket/TCP/__init__.py
--rw-r--r--   0        0        0     6872 2023-09-27 14:46:56.704276 bagbag-0.67.2/src/bagbag/Socket/TCP/src.py
--rw-r--r--   0        0        0      441 2024-01-18 07:54:49.902363 bagbag-0.67.2/src/bagbag/Socket/UDP/__init__.py
--rw-r--r--   0        0        0     2626 2024-01-18 08:41:32.180827 bagbag-0.67.2/src/bagbag/Socket/UDP/src.py
--rw-r--r--   0        0        0       35 2024-01-18 08:13:19.939955 bagbag-0.67.2/src/bagbag/Socket/__init__.py
--rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.67.2/src/bagbag/String/__init__.py
--rw-r--r--   0        0        0    17934 2024-05-09 02:10:18.454205 bagbag-0.67.2/src/bagbag/String/src.py
--rw-r--r--   0        0        0    17050 2024-05-09 02:09:30.442101 bagbag-0.67.2/src/bagbag/String/tlds.txt
--rw-r--r--   0        0        0    26594 2023-07-30 08:54:20.166240 bagbag-0.67.2/src/bagbag/String/vars.py
--rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.67.2/src/bagbag/Thread/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-15 09:24:51.853905 bagbag-0.67.2/src/bagbag/Thread/src.py
--rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.67.2/src/bagbag/Time/__init__.py
--rw-r--r--   0        0        0     6062 2024-02-24 01:15:02.116565 bagbag-0.67.2/src/bagbag/Time/src.py
--rw-r--r--   0        0        0     2450 2023-09-22 09:26:44.680152 bagbag-0.67.2/src/bagbag/Tools/Argparser_src.py
--rw-r--r--   0        0        0     2614 2023-09-22 09:26:44.687575 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
--rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
--rw-r--r--   0        0        0      973 2023-09-22 09:26:44.687563 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
--rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/__init__.py
--rw-r--r--   0        0        0      461 2023-08-14 09:09:47.622480 bagbag-0.67.2/src/bagbag/Tools/BlockChain/CoinMarketCap/__init__.py
--rw-r--r--   0        0        0     6687 2023-08-16 09:02:48.339339 bagbag-0.67.2/src/bagbag/Tools/BlockChain/CoinMarketCap/api.py
--rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
--rw-r--r--   0        0        0      326 2023-09-22 09:26:44.687610 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
--rw-r--r--   0        0        0     1421 2023-08-20 06:15:23.885306 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Others/FearAndGreedIndex_src.py
--rw-r--r--   0        0        0      392 2023-08-20 06:02:39.845710 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Others/__init__.py
--rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Tron/__init__.py
--rw-r--r--   0        0        0    24278 2023-09-22 09:26:44.687599 bagbag-0.67.2/src/bagbag/Tools/BlockChain/Tron/src.py
--rw-r--r--   0        0        0      505 2023-08-20 06:03:16.531548 bagbag-0.67.2/src/bagbag/Tools/BlockChain/__init__.py
--rw-r--r--   0        0        0     3278 2023-09-22 09:26:44.687348 bagbag-0.67.2/src/bagbag/Tools/CSV.py
--rw-r--r--   0        0        0     4616 2023-09-22 09:26:44.687312 bagbag-0.67.2/src/bagbag/Tools/Cache.py
--rw-r--r--   0        0        0     3901 2024-04-10 07:38:42.872848 bagbag-0.67.2/src/bagbag/Tools/Chan_src.py
--rw-r--r--   0        0        0    32942 2023-09-22 09:26:44.680139 bagbag-0.67.2/src/bagbag/Tools/ComputerVision.py
--rw-r--r--   0        0        0     3239 2023-09-22 09:26:44.672681 bagbag-0.67.2/src/bagbag/Tools/Crontab_src.py
--rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.67.2/src/bagbag/Tools/Database/__init__.py
--rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.67.2/src/bagbag/Tools/Database/orator/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/__init__.py
--rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/application.py
--rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/command.py
--rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
--rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
--rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
--rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
--rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
--rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
--rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
--rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
--rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/models/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/models/make_command.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/models/stubs.py
--rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
--rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
--rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
--rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/__init__.py
--rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/connection.py
--rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/connection_interface.py
--rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
--rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
--rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
--rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
--rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/__init__.py
--rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
--rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/connector.py
--rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
--rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
--rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
--rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.67.2/src/bagbag/Tools/Database/orator/database_manager.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/__init__.py
--rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
--rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/column.py
--rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/column_diff.py
--rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/comparator.py
--rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
--rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
--rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/identifier.py
--rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/index.py
--rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
--rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
--rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
--rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
--rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
--rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
--rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
--rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
--rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
--rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
--rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
--rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
--rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
--rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/table.py
--rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/table_diff.py
--rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
--rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.67.2/src/bagbag/Tools/Database/orator/events/__init__.py
--rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/__init__.py
--rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/connection.py
--rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/connectors.py
--rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/orm.py
--rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/query.py
--rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/__init__.py
--rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
--rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/migration.py
--rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
--rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/migrator.py
--rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/stubs.py
--rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/__init__.py
--rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/builder.py
--rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/collection.py
--rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/factory.py
--rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/factory_builder.py
--rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
--rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
--rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/model.py
--rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
--rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
--rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
--rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
--rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
--rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
--rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
--rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
--rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
--rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
--rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
--rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
--rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
--rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
--rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/relation.py
--rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/result.py
--rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
--rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
--rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
--rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
--rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/utils.py
--rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/__init__.py
--rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/base.py
--rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
--rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/paginator.py
--rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/__init__.py
--rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/builder.py
--rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/expression.py
--rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
--rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
--rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/join_clause.py
--rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/__init__.py
--rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
--rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
--rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/processor.py
--rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
--rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/__init__.py
--rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/blueprint.py
--rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/builder.py
--rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
--rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
--rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
--rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
--rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
--rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
--rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/schema.py
--rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.67.2/src/bagbag/Tools/Database/orator/seeds/__init__.py
--rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.67.2/src/bagbag/Tools/Database/orator/seeds/seeder.py
--rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.67.2/src/bagbag/Tools/Database/orator/seeds/stubs.py
--rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/__init__.py
--rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/collection.py
--rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/fluent.py
--rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/grammar.py
--rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/__init__.py
--rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/command_formatter.py
--rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/helpers.py
--rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/qmarker.py
--rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/url.py
--rw-r--r--   0        0        0    33893 2023-10-18 14:56:35.779826 bagbag-0.67.2/src/bagbag/Tools/Database/src.py
--rw-r--r--   0        0        0     5251 2023-09-22 09:26:44.680084 bagbag-0.67.2/src/bagbag/Tools/DistributedLock_src.py
--rw-r--r--   0        0        0     6759 2024-02-24 09:29:11.920490 bagbag-0.67.2/src/bagbag/Tools/Elasticsearch_src.py
--rw-r--r--   0        0        0     4313 2023-09-22 09:26:44.687329 bagbag-0.67.2/src/bagbag/Tools/Github_src.py
--rw-r--r--   0        0        0     1452 2023-09-22 09:26:44.687245 bagbag-0.67.2/src/bagbag/Tools/JavaScript_src.py
--rw-r--r--   0        0        0    11103 2024-01-26 06:39:30.192158 bagbag-0.67.2/src/bagbag/Tools/Kafka_src.py
--rw-r--r--   0        0        0     2029 2023-09-22 09:26:44.633507 bagbag-0.67.2/src/bagbag/Tools/Lock_src.py
--rw-r--r--   0        0        0     6635 2023-09-22 09:26:44.687412 bagbag-0.67.2/src/bagbag/Tools/MatrixBot_src.py
--rw-r--r--   0        0        0     1510 2024-01-12 08:41:39.736400 bagbag-0.67.2/src/bagbag/Tools/Nslookup_src.py
--rw-r--r--   0        0        0     2365 2023-09-22 09:26:44.673022 bagbag-0.67.2/src/bagbag/Tools/OCR_src.py
--rw-r--r--   0        0        0     3607 2024-05-10 12:51:32.811252 bagbag-0.67.2/src/bagbag/Tools/OpenAI.py
--rw-r--r--   0        0        0     3716 2024-01-14 07:33:09.943287 bagbag-0.67.2/src/bagbag/Tools/ProgressBar_src.py
--rw-r--r--   0        0        0     1661 2023-09-22 09:26:44.687535 bagbag-0.67.2/src/bagbag/Tools/Prometheus/MetricServer.py
--rw-r--r--   0        0        0     3518 2024-02-02 03:59:39.001962 bagbag-0.67.2/src/bagbag/Tools/Prometheus/PushGateway.py
--rw-r--r--   0        0        0      177 2024-01-15 06:37:19.255853 bagbag-0.67.2/src/bagbag/Tools/Prometheus/Utils.py
--rw-r--r--   0        0        0      157 2024-01-15 06:36:14.708912 bagbag-0.67.2/src/bagbag/Tools/Prometheus/__init__.py
--rw-r--r--   0        0        0     4750 2024-02-20 03:07:14.267082 bagbag-0.67.2/src/bagbag/Tools/Prometheus/metrics.py
--rw-r--r--   0        0        0     2608 2023-09-22 09:26:44.680110 bagbag-0.67.2/src/bagbag/Tools/Queue_src.py
--rw-r--r--   0        0        0     2491 2023-09-22 09:26:44.687633 bagbag-0.67.2/src/bagbag/Tools/RSS/Feed_src.py
--rw-r--r--   0        0        0      662 2023-09-22 09:26:44.687624 bagbag-0.67.2/src/bagbag/Tools/RSS/Opml_src.py
--rw-r--r--   0        0        0      619 2023-08-23 16:03:38.456528 bagbag-0.67.2/src/bagbag/Tools/RSS/__init__.py
--rw-r--r--   0        0        0     3689 2023-09-22 09:26:44.572324 bagbag-0.67.2/src/bagbag/Tools/Ratelimit_src.py
--rw-r--r--   0        0        0    26542 2024-05-08 06:59:03.274855 bagbag-0.67.2/src/bagbag/Tools/Redis_src.py
--rw-r--r--   0        0        0     7168 2024-01-22 04:19:19.682899 bagbag-0.67.2/src/bagbag/Tools/SMTP_src.py
--rw-r--r--   0        0        0     5610 2023-09-22 09:26:44.672664 bagbag-0.67.2/src/bagbag/Tools/SSH_src.py
--rw-r--r--   0        0        0    35116 2023-09-22 09:26:44.687431 bagbag-0.67.2/src/bagbag/Tools/Selenium.py
--rw-r--r--   0        0        0    14132 2023-09-22 09:26:44.680059 bagbag-0.67.2/src/bagbag/Tools/TelegramAsync.py
--rw-r--r--   0        0        0     5112 2023-09-22 09:26:44.697272 bagbag-0.67.2/src/bagbag/Tools/TelegramBotOfficial_src.py
--rw-r--r--   0        0        0     3070 2023-09-22 09:26:44.687395 bagbag-0.67.2/src/bagbag/Tools/TelegramBot_src.py
--rw-r--r--   0        0        0    25972 2023-11-15 06:42:20.918334 bagbag-0.67.2/src/bagbag/Tools/Telegram_src.py
--rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.67.2/src/bagbag/Tools/Test.py
--rw-r--r--   0        0        0     3330 2023-07-30 16:03:16.992060 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/Bayes.py
--rw-r--r--   0        0        0     3360 2023-07-30 16:04:55.755050 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/LogisticRegression.py
--rw-r--r--   0        0        0     4443 2023-07-30 16:01:37.360637 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/SVM.py
--rw-r--r--   0        0        0       96 2023-07-30 15:32:40.319669 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/__init__.py
--rw-r--r--   0        0        0     6529 2023-09-22 09:26:44.687816 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/base.py
--rw-r--r--   0        0        0    24552 2023-07-30 08:53:13.297800 bagbag-0.67.2/src/bagbag/Tools/TextClassifier/vars.py
--rw-r--r--   0        0        0     4817 2023-09-22 09:26:44.687451 bagbag-0.67.2/src/bagbag/Tools/Translater.py
--rw-r--r--   0        0        0    14103 2023-06-19 07:22:24.505061 bagbag-0.67.2/src/bagbag/Tools/Twitter/Browser_src.py
--rw-r--r--   0        0        0    12719 2023-09-22 09:26:44.697186 bagbag-0.67.2/src/bagbag/Tools/Twitter/Elevated_src.py
--rw-r--r--   0        0        0     2094 2023-09-22 09:26:44.687644 bagbag-0.67.2/src/bagbag/Tools/Twitter/Essential_src.py
--rw-r--r--   0        0        0    29455 2023-08-03 11:34:20.274523 bagbag-0.67.2/src/bagbag/Tools/Twitter/Nitter_src.py
--rw-r--r--   0        0        0     2744 2023-06-16 08:15:42.223073 bagbag-0.67.2/src/bagbag/Tools/Twitter/Utils.py
--rw-r--r--   0        0        0     1070 2023-07-19 12:53:41.487474 bagbag-0.67.2/src/bagbag/Tools/Twitter/__init__.py
--rw-r--r--   0        0        0     3298 2023-09-22 09:26:44.672824 bagbag-0.67.2/src/bagbag/Tools/URL_src.py
--rw-r--r--   0        0        0      768 2023-09-22 09:26:44.680096 bagbag-0.67.2/src/bagbag/Tools/WaitGroup_src.py
--rw-r--r--   0        0        0     8127 2023-09-22 09:26:44.687287 bagbag-0.67.2/src/bagbag/Tools/WebCrawler_src.py
--rw-r--r--   0        0        0     7210 2024-04-09 13:05:04.493796 bagbag-0.67.2/src/bagbag/Tools/WebServer_src.py
--rw-r--r--   0        0        0     3467 2023-12-15 09:08:11.884051 bagbag-0.67.2/src/bagbag/Tools/XPath_src.py
--rw-r--r--   0        0        0     3236 2023-09-22 09:26:44.572163 bagbag-0.67.2/src/bagbag/Tools/Xlsx.py
--rw-r--r--   0        0        0     3754 2024-04-11 02:15:29.230060 bagbag-0.67.2/src/bagbag/Tools/__init__.py
--rw-r--r--   0        0        0     9404 2023-09-07 06:44:18.178279 bagbag-0.67.2/src/bagbag/Tools/pygtrans/ApiKeyTranslate.py
--rw-r--r--   0        0        0      664 2023-09-07 06:44:18.178362 bagbag-0.67.2/src/bagbag/Tools/pygtrans/DetectResponse.py
--rw-r--r--   0        0        0      424 2023-09-07 06:44:18.178562 bagbag-0.67.2/src/bagbag/Tools/pygtrans/LanguageResponse.py
--rw-r--r--   0        0        0      418 2023-09-07 06:44:18.178627 bagbag-0.67.2/src/bagbag/Tools/pygtrans/Null.py
--rw-r--r--   0        0        0     8717 2023-09-07 06:45:37.193201 bagbag-0.67.2/src/bagbag/Tools/pygtrans/Translate.py
--rw-r--r--   0        0        0     1238 2023-09-07 06:44:18.178758 bagbag-0.67.2/src/bagbag/Tools/pygtrans/TranslateResponse.py
--rw-r--r--   0        0        0      710 2023-09-07 06:44:18.178865 bagbag-0.67.2/src/bagbag/Tools/pygtrans/__init__.py
--rw-r--r--   0        0        0     4560 2023-10-18 11:53:05.137309 bagbag-0.67.2/src/bagbag/__init__.py
--rw-r--r--   0        0        0    20049 1970-01-01 00:00:00.000000 bagbag-0.67.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-07-07 19:24:15.851188 bagbag-0.67.3/LICENSE
+-rw-r--r--   0        0        0    16842 2023-06-09 06:25:43.991924 bagbag-0.67.3/README.md
+-rw-r--r--   0        0        0     2416 2024-05-11 01:55:18.160132 bagbag-0.67.3/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-05-12 12:35:25.861360 bagbag-0.67.3/src/bagbag/Base64/__init__.py
+-rw-r--r--   0        0        0      480 2023-09-22 09:26:09.030151 bagbag-0.67.3/src/bagbag/Base64/src.py
+-rw-r--r--   0        0        0      561 2023-08-29 18:20:15.861931 bagbag-0.67.3/src/bagbag/Cmd/__init__.py
+-rw-r--r--   0        0        0     5946 2024-01-08 10:23:15.811164 bagbag-0.67.3/src/bagbag/Cmd/src.py
+-rw-r--r--   0        0        0      361 2023-05-12 12:35:25.866128 bagbag-0.67.3/src/bagbag/Cryptoo/__init__.py
+-rw-r--r--   0        0        0     2539 2023-09-22 09:26:44.572415 bagbag-0.67.3/src/bagbag/Cryptoo/src.py
+-rw-r--r--   0        0        0      348 2023-06-02 17:02:39.723337 bagbag-0.67.3/src/bagbag/File/__init__.py
+-rw-r--r--   0        0        0     5162 2023-08-18 05:52:04.823383 bagbag-0.67.3/src/bagbag/File/src.py
+-rw-r--r--   0        0        0    16724 2023-05-12 12:35:25.857941 bagbag-0.67.3/src/bagbag/Funcs/CutSentenceStopWords_src.py
+-rw-r--r--   0        0        0      858 2023-09-22 09:26:44.571988 bagbag-0.67.3/src/bagbag/Funcs/CutSentence_src.py
+-rw-r--r--   0        0        0     6833 2023-09-22 09:26:44.572042 bagbag-0.67.3/src/bagbag/Funcs/FakeIdentity_src.py
+-rw-r--r--   0        0        0      558 2023-09-22 09:26:44.571998 bagbag-0.67.3/src/bagbag/Funcs/FileType_src.py
+-rw-r--r--   0        0        0      389 2023-05-12 12:35:25.858488 bagbag-0.67.3/src/bagbag/Funcs/Format/__init__.py
+-rw-r--r--   0        0        0      837 2023-09-22 09:26:44.572060 bagbag-0.67.3/src/bagbag/Funcs/Format/src.py
+-rw-r--r--   0        0        0      753 2023-09-22 09:26:44.571981 bagbag-0.67.3/src/bagbag/Funcs/GetPublicIP_src.py
+-rw-r--r--   0        0        0      296 2023-09-22 09:26:44.572371 bagbag-0.67.3/src/bagbag/Funcs/IPAddressConvert_src.py
+-rw-r--r--   0        0        0      474 2023-09-22 09:26:44.572073 bagbag-0.67.3/src/bagbag/Funcs/Markdown_src.py
+-rw-r--r--   0        0        0      996 2023-09-22 09:26:44.571956 bagbag-0.67.3/src/bagbag/Funcs/Ping_src.py
+-rw-r--r--   0        0        0     1730 2023-09-22 09:26:44.571972 bagbag-0.67.3/src/bagbag/Funcs/ResizeImage_src.py
+-rw-r--r--   0        0        0      181 2023-11-01 18:01:37.175603 bagbag-0.67.3/src/bagbag/Funcs/UUID_src.py
+-rw-r--r--   0        0        0      511 2024-01-10 05:42:03.100032 bagbag-0.67.3/src/bagbag/Funcs/VersionCompare_src.py
+-rw-r--r--   0        0        0     1458 2023-09-22 09:26:44.572132 bagbag-0.67.3/src/bagbag/Funcs/Wget_src.py
+-rw-r--r--   0        0        0      219 2024-05-09 06:52:12.594416 bagbag-0.67.3/src/bagbag/Funcs/Whois_src.py
+-rw-r--r--   0        0        0     1336 2024-05-09 06:40:19.129474 bagbag-0.67.3/src/bagbag/Funcs/__init__.py
+-rw-r--r--   0        0        0     5364 2024-05-09 06:35:52.807587 bagbag-0.67.3/src/bagbag/Funcs/whois/__init__.py
+-rw-r--r--   0        0        0   232589 2024-05-09 06:35:52.808013 bagbag-0.67.3/src/bagbag/Funcs/whois/data/public_suffix_list.dat
+-rw-r--r--   0        0        0   127805 2024-05-09 06:53:24.503036 bagbag-0.67.3/src/bagbag/Funcs/whois/parser.py
+-rw-r--r--   0        0        0     1518 2024-05-09 06:35:52.808434 bagbag-0.67.3/src/bagbag/Funcs/whois/time_zones.py
+-rw-r--r--   0        0        0    15439 2024-05-09 06:35:52.808590 bagbag-0.67.3/src/bagbag/Funcs/whois/whois.py
+-rw-r--r--   0        0        0      577 2023-05-12 12:35:25.862318 bagbag-0.67.3/src/bagbag/Hash/__init__.py
+-rw-r--r--   0        0        0     1451 2023-09-22 09:26:44.572298 bagbag-0.67.3/src/bagbag/Hash/src.py
+-rw-r--r--   0        0        0      683 2023-05-12 12:35:25.862782 bagbag-0.67.3/src/bagbag/Http/__init__.py
+-rw-r--r--   0        0        0    12346 2023-09-22 09:26:44.571920 bagbag-0.67.3/src/bagbag/Http/src.py
+-rw-r--r--   0        0        0      418 2023-05-12 12:35:25.863142 bagbag-0.67.3/src/bagbag/Json/__init__.py
+-rw-r--r--   0        0        0     3272 2023-09-22 09:26:44.572028 bagbag-0.67.3/src/bagbag/Json/src.py
+-rw-r--r--   0        0        0    10860 2023-06-16 14:21:52.035937 bagbag-0.67.3/src/bagbag/Lg.py
+-rw-r--r--   0        0        0      382 2023-05-12 12:35:25.863851 bagbag-0.67.3/src/bagbag/Math/__init__.py
+-rw-r--r--   0        0        0     2076 2023-09-22 09:26:44.572144 bagbag-0.67.3/src/bagbag/Math/src.py
+-rw-r--r--   0        0        0      639 2023-05-15 13:18:35.454738 bagbag-0.67.3/src/bagbag/Os/Path/__init__.py
+-rw-r--r--   0        0        0     1889 2023-09-22 09:26:44.571833 bagbag-0.67.3/src/bagbag/Os/Path/src.py
+-rw-r--r--   0        0        0     1047 2023-09-29 15:45:37.749849 bagbag-0.67.3/src/bagbag/Os/__init__.py
+-rw-r--r--   0        0        0     3468 2023-09-29 15:42:54.859953 bagbag-0.67.3/src/bagbag/Os/src.py
+-rw-r--r--   0        0        0      354 2023-05-12 12:35:25.864309 bagbag-0.67.3/src/bagbag/Process/__init__.py
+-rw-r--r--   0        0        0     1239 2023-06-15 09:27:23.720590 bagbag-0.67.3/src/bagbag/Process/src.py
+-rw-r--r--   0        0        0      447 2023-10-18 11:52:42.930164 bagbag-0.67.3/src/bagbag/Python/__init__.py
+-rw-r--r--   0        0        0     1650 2023-11-05 14:21:13.197206 bagbag-0.67.3/src/bagbag/Python/src.py
+-rw-r--r--   0        0        0      464 2023-05-12 12:35:25.865128 bagbag-0.67.3/src/bagbag/Random/__init__.py
+-rw-r--r--   0        0        0      817 2024-01-12 08:21:43.555903 bagbag-0.67.3/src/bagbag/Random/src.py
+-rw-r--r--   0        0        0      510 2023-07-19 13:13:12.245619 bagbag-0.67.3/src/bagbag/Socket/TCP/__init__.py
+-rw-r--r--   0        0        0     6872 2023-09-27 14:46:56.704276 bagbag-0.67.3/src/bagbag/Socket/TCP/src.py
+-rw-r--r--   0        0        0      441 2024-01-18 07:54:49.902363 bagbag-0.67.3/src/bagbag/Socket/UDP/__init__.py
+-rw-r--r--   0        0        0     2626 2024-01-18 08:41:32.180827 bagbag-0.67.3/src/bagbag/Socket/UDP/src.py
+-rw-r--r--   0        0        0       35 2024-01-18 08:13:19.939955 bagbag-0.67.3/src/bagbag/Socket/__init__.py
+-rw-r--r--   0        0        0      352 2023-05-12 12:35:25.865416 bagbag-0.67.3/src/bagbag/String/__init__.py
+-rw-r--r--   0        0        0    17934 2024-05-09 02:10:18.454205 bagbag-0.67.3/src/bagbag/String/src.py
+-rw-r--r--   0        0        0    17050 2024-05-09 02:09:30.442101 bagbag-0.67.3/src/bagbag/String/tlds.txt
+-rw-r--r--   0        0        0    26594 2023-07-30 08:54:20.166240 bagbag-0.67.3/src/bagbag/String/vars.py
+-rw-r--r--   0        0        0      367 2023-05-12 12:35:25.865783 bagbag-0.67.3/src/bagbag/Thread/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-15 09:24:51.853905 bagbag-0.67.3/src/bagbag/Thread/src.py
+-rw-r--r--   0        0        0      571 2023-06-15 06:22:08.764134 bagbag-0.67.3/src/bagbag/Time/__init__.py
+-rw-r--r--   0        0        0     6062 2024-02-24 01:15:02.116565 bagbag-0.67.3/src/bagbag/Time/src.py
+-rw-r--r--   0        0        0     2450 2023-09-22 09:26:44.680152 bagbag-0.67.3/src/bagbag/Tools/Argparser_src.py
+-rw-r--r--   0        0        0     2614 2023-09-22 09:26:44.687575 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py
+-rw-r--r--   0        0        0      350 2023-05-12 12:35:25.826469 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/__init__.py
+-rw-r--r--   0        0        0      973 2023-09-22 09:26:44.687563 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py
+-rw-r--r--   0        0        0      509 2023-05-12 12:35:25.825419 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/__init__.py
+-rw-r--r--   0        0        0      461 2023-08-14 09:09:47.622480 bagbag-0.67.3/src/bagbag/Tools/BlockChain/CoinMarketCap/__init__.py
+-rw-r--r--   0        0        0     6687 2023-08-16 09:02:48.339339 bagbag-0.67.3/src/bagbag/Tools/BlockChain/CoinMarketCap/api.py
+-rw-r--r--   0        0        0       36 2023-05-12 12:35:25.827257 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Ethereum/__init__.py
+-rw-r--r--   0        0        0      326 2023-09-22 09:26:44.687610 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Ethereum/ethereum.py
+-rw-r--r--   0        0        0     1421 2023-08-20 06:15:23.885306 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Others/FearAndGreedIndex_src.py
+-rw-r--r--   0        0        0      392 2023-08-20 06:02:39.845710 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Others/__init__.py
+-rw-r--r--   0        0        0      485 2023-05-12 12:35:25.824938 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Tron/__init__.py
+-rw-r--r--   0        0        0    24278 2023-09-22 09:26:44.687599 bagbag-0.67.3/src/bagbag/Tools/BlockChain/Tron/src.py
+-rw-r--r--   0        0        0      505 2023-08-20 06:03:16.531548 bagbag-0.67.3/src/bagbag/Tools/BlockChain/__init__.py
+-rw-r--r--   0        0        0     3278 2023-09-22 09:26:44.687348 bagbag-0.67.3/src/bagbag/Tools/CSV.py
+-rw-r--r--   0        0        0     4616 2023-09-22 09:26:44.687312 bagbag-0.67.3/src/bagbag/Tools/Cache.py
+-rw-r--r--   0        0        0     3901 2024-04-10 07:38:42.872848 bagbag-0.67.3/src/bagbag/Tools/Chan_src.py
+-rw-r--r--   0        0        0    32942 2023-09-22 09:26:44.680139 bagbag-0.67.3/src/bagbag/Tools/ComputerVision.py
+-rw-r--r--   0        0        0     3239 2023-09-22 09:26:44.672681 bagbag-0.67.3/src/bagbag/Tools/Crontab_src.py
+-rw-r--r--   0        0        0      644 2023-05-12 12:35:25.856714 bagbag-0.67.3/src/bagbag/Tools/Database/__init__.py
+-rw-r--r--   0        0        0      297 2023-05-12 12:35:25.830525 bagbag-0.67.3/src/bagbag/Tools/Database/orator/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.830659 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/__init__.py
+-rw-r--r--   0        0        0      785 2023-05-12 12:35:25.830739 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/application.py
+-rw-r--r--   0        0        0     3436 2023-05-12 12:35:25.830822 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/command.py
+-rw-r--r--   0        0        0      330 2023-05-12 12:35:25.830964 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/__init__.py
+-rw-r--r--   0        0        0      186 2023-05-12 12:35:25.831040 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/base_command.py
+-rw-r--r--   0        0        0      626 2023-05-12 12:35:25.831123 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py
+-rw-r--r--   0        0        0     1301 2023-05-12 12:35:25.831226 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py
+-rw-r--r--   0        0        0     2343 2023-05-12 12:35:25.831313 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py
+-rw-r--r--   0        0        0     1886 2023-05-12 12:35:25.831395 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py
+-rw-r--r--   0        0        0     1308 2023-05-12 12:35:25.831488 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py
+-rw-r--r--   0        0        0     1315 2023-05-12 12:35:25.831583 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py
+-rw-r--r--   0        0        0     1642 2023-05-12 12:35:25.831666 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.831798 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/models/__init__.py
+-rw-r--r--   0        0        0     2217 2023-05-12 12:35:25.831874 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/models/make_command.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.831968 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/models/stubs.py
+-rw-r--r--   0        0        0      108 2023-05-12 12:35:25.832158 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/__init__.py
+-rw-r--r--   0        0        0      178 2023-05-12 12:35:25.832248 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/base_command.py
+-rw-r--r--   0        0        0     2204 2023-05-12 12:35:25.832352 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py
+-rw-r--r--   0        0        0     1923 2023-05-12 12:35:25.832446 bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.832590 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/__init__.py
+-rw-r--r--   0        0        0    15063 2023-05-12 12:35:25.832673 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/connection.py
+-rw-r--r--   0        0        0     4112 2023-05-12 12:35:25.832759 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/connection_interface.py
+-rw-r--r--   0        0        0      298 2023-05-12 12:35:25.832861 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/connection_resolver_interface.py
+-rw-r--r--   0        0        0     2218 2023-05-12 12:35:25.832962 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/mysql_connection.py
+-rw-r--r--   0        0        0     2056 2023-05-12 12:35:25.833055 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/postgres_connection.py
+-rw-r--r--   0        0        0     1588 2023-05-12 12:35:25.833159 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py
+-rw-r--r--   0        0        0      198 2023-05-12 12:35:25.833971 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/__init__.py
+-rw-r--r--   0        0        0     3133 2023-05-12 12:35:25.834056 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/connection_factory.py
+-rw-r--r--   0        0        0     3106 2023-05-12 12:35:25.834129 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/connector.py
+-rw-r--r--   0        0        0     3982 2023-05-12 12:35:25.834204 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py
+-rw-r--r--   0        0        0     3280 2023-05-12 12:35:25.834291 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py
+-rw-r--r--   0        0        0     2172 2023-05-12 12:35:25.834370 bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py
+-rw-r--r--   0        0        0     5089 2023-05-12 12:35:25.835189 bagbag-0.67.3/src/bagbag/Tools/Database/orator/database_manager.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.835796 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-12 12:35:25.835903 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py
+-rw-r--r--   0        0        0     3447 2023-05-12 12:35:25.835999 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/column.py
+-rw-r--r--   0        0        0      545 2023-05-12 12:35:25.836087 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/column_diff.py
+-rw-r--r--   0        0        0    11219 2023-05-12 12:35:25.836174 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/comparator.py
+-rw-r--r--   0        0        0     1943 2023-05-12 12:35:25.836319 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py
+-rw-r--r--   0        0        0     8193 2023-05-12 12:35:25.836678 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py
+-rw-r--r--   0        0        0      173 2023-05-12 12:35:25.836774 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/identifier.py
+-rw-r--r--   0        0        0     7094 2023-05-12 12:35:25.836858 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/index.py
+-rw-r--r--   0        0        0     5260 2023-05-12 12:35:25.836935 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py
+-rw-r--r--   0        0        0      205 2023-05-12 12:35:25.837074 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/__init__.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.837217 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-12 12:35:25.837297 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/keyword_list.py
+-rw-r--r--   0        0        0     4383 2023-05-12 12:35:25.837375 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.837455 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py
+-rw-r--r--   0        0        0     2315 2023-05-12 12:35:25.837531 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py
+-rw-r--r--   0        0        0     1289 2023-05-12 12:35:25.838118 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py
+-rw-r--r--   0        0        0     9489 2023-05-12 12:35:25.838202 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py
+-rw-r--r--   0        0        0    21672 2023-05-12 12:35:25.838290 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py
+-rw-r--r--   0        0        0    14126 2023-05-12 12:35:25.838370 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py
+-rw-r--r--   0        0        0    20833 2023-05-12 12:35:25.838457 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py
+-rw-r--r--   0        0        0     6014 2023-05-12 12:35:25.839154 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py
+-rw-r--r--   0        0        0     4240 2023-05-12 12:35:25.839242 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/schema_manager.py
+-rw-r--r--   0        0        0     5458 2023-05-12 12:35:25.839325 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py
+-rw-r--r--   0        0        0    17146 2023-05-12 12:35:25.839403 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/table.py
+-rw-r--r--   0        0        0     1436 2023-05-12 12:35:25.839495 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/table_diff.py
+-rw-r--r--   0        0        0       24 2023-05-12 12:35:25.839639 bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/types/__init__.py
+-rw-r--r--   0        0        0      992 2023-05-12 12:35:25.840999 bagbag-0.67.3/src/bagbag/Tools/Database/orator/events/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-12 12:35:25.841361 bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/__init__.py
+-rw-r--r--   0        0        0      193 2023-05-12 12:35:25.841461 bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/connection.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:35:25.841563 bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/connectors.py
+-rw-r--r--   0        0        0      551 2023-05-12 12:35:25.841649 bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/orm.py
+-rw-r--r--   0        0        0      494 2023-05-12 12:35:25.841746 bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/query.py
+-rw-r--r--   0        0        0      208 2023-05-12 12:35:25.842330 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/__init__.py
+-rw-r--r--   0        0        0     2730 2023-05-12 12:35:25.842410 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py
+-rw-r--r--   0        0        0      425 2023-05-12 12:35:25.842506 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/migration.py
+-rw-r--r--   0        0        0     2588 2023-05-12 12:35:25.842583 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/migration_creator.py
+-rw-r--r--   0        0        0     7754 2023-05-12 12:35:25.842660 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/migrator.py
+-rw-r--r--   0        0        0     1114 2023-05-12 12:35:25.842735 bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/stubs.py
+-rw-r--r--   0        0        0      419 2023-05-12 12:35:25.842873 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/__init__.py
+-rw-r--r--   0        0        0    32311 2023-05-12 12:35:25.842946 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/builder.py
+-rw-r--r--   0        0        0      814 2023-05-12 12:35:25.843014 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/collection.py
+-rw-r--r--   0        0        0     7481 2023-05-12 12:35:25.843112 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/factory.py
+-rw-r--r--   0        0        0     2579 2023-05-12 12:35:25.843207 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/factory_builder.py
+-rw-r--r--   0        0        0       63 2023-05-12 12:35:25.843408 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/mixins/__init__.py
+-rw-r--r--   0        0        0     3532 2023-05-12 12:35:25.843502 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py
+-rw-r--r--   0        0        0    75367 2023-05-12 12:35:25.843880 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/model.py
+-rw-r--r--   0        0        0      371 2023-05-12 12:35:25.844072 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/__init__.py
+-rw-r--r--   0        0        0     5427 2023-05-12 12:35:25.844163 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py
+-rw-r--r--   0        0        0    23248 2023-05-12 12:35:25.844271 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py
+-rw-r--r--   0        0        0     1012 2023-05-12 12:35:25.844373 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_many.py
+-rw-r--r--   0        0        0     5126 2023-05-12 12:35:25.844473 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py
+-rw-r--r--   0        0        0      955 2023-05-12 12:35:25.844558 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_one.py
+-rw-r--r--   0        0        0     8617 2023-05-12 12:35:25.844637 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py
+-rw-r--r--   0        0        0      899 2023-05-12 12:35:25.844716 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py
+-rw-r--r--   0        0        0      843 2023-05-12 12:35:25.844810 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py
+-rw-r--r--   0        0        0     5377 2023-05-12 12:35:25.844920 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py
+-rw-r--r--   0        0        0      984 2023-05-12 12:35:25.845022 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py
+-rw-r--r--   0        0        0     5293 2023-05-12 12:35:25.845127 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py
+-rw-r--r--   0        0        0     3555 2023-05-12 12:35:25.845220 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py
+-rw-r--r--   0        0        0     2978 2023-05-12 12:35:25.845313 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/pivot.py
+-rw-r--r--   0        0        0     5956 2023-05-12 12:35:25.845401 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/relation.py
+-rw-r--r--   0        0        0      685 2023-05-12 12:35:25.845502 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/result.py
+-rw-r--r--   0        0        0     1106 2023-05-12 12:35:25.845583 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py
+-rw-r--r--   0        0        0       95 2023-05-12 12:35:25.847154 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/scopes/__init__.py
+-rw-r--r--   0        0        0      348 2023-05-12 12:35:25.847229 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/scopes/scope.py
+-rw-r--r--   0        0        0     3900 2023-05-12 12:35:25.847308 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py
+-rw-r--r--   0        0        0    13642 2023-05-12 12:35:25.847743 bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/utils.py
+-rw-r--r--   0        0        0      115 2023-05-12 12:35:25.848559 bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-12 12:35:25.848628 bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/base.py
+-rw-r--r--   0        0        0     2426 2023-05-12 12:35:25.848698 bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py
+-rw-r--r--   0        0        0     2216 2023-05-12 12:35:25.848764 bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/paginator.py
+-rw-r--r--   0        0        0       59 2023-05-12 12:35:25.849247 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/__init__.py
+-rw-r--r--   0        0        0    44030 2023-05-12 12:35:25.849322 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/builder.py
+-rw-r--r--   0        0        0      230 2023-05-12 12:35:25.849403 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/expression.py
+-rw-r--r--   0        0        0      202 2023-05-12 12:35:25.849583 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/__init__.py
+-rw-r--r--   0        0        0    13999 2023-05-12 12:35:25.849662 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/grammar.py
+-rw-r--r--   0        0        0     3559 2023-05-12 12:35:25.849810 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     4461 2023-05-12 12:35:25.849897 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     4204 2023-05-12 12:35:25.849974 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1407 2023-05-12 12:35:25.850460 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/join_clause.py
+-rw-r--r--   0        0        0      218 2023-05-12 12:35:25.850604 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-12 12:35:25.850669 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py
+-rw-r--r--   0        0        0     1160 2023-05-12 12:35:25.850732 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py
+-rw-r--r--   0        0        0     1423 2023-05-12 12:35:25.850798 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/processor.py
+-rw-r--r--   0        0        0      422 2023-05-12 12:35:25.850863 bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/sqlite_processor.py
+-rw-r--r--   0        0        0      166 2023-05-12 12:35:25.851787 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/__init__.py
+-rw-r--r--   0        0        0    19482 2023-05-12 12:35:25.851871 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/blueprint.py
+-rw-r--r--   0        0        0     3617 2023-05-12 12:35:25.851961 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/builder.py
+-rw-r--r--   0        0        0      206 2023-05-12 12:35:25.852130 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/__init__.py
+-rw-r--r--   0        0        0     9880 2023-05-12 12:35:25.852215 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py
+-rw-r--r--   0        0        0     8503 2023-05-12 12:35:25.852316 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py
+-rw-r--r--   0        0        0     7103 2023-05-12 12:35:25.852415 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py
+-rw-r--r--   0        0        0     8321 2023-05-12 12:35:25.852524 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py
+-rw-r--r--   0        0        0     1229 2023-05-12 12:35:25.853214 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/mysql_builder.py
+-rw-r--r--   0        0        0      645 2023-05-12 12:35:25.853314 bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/schema.py
+-rw-r--r--   0        0        0       52 2023-05-12 12:35:25.854121 bagbag-0.67.3/src/bagbag/Tools/Database/orator/seeds/__init__.py
+-rw-r--r--   0        0        0     1730 2023-05-12 12:35:25.854207 bagbag-0.67.3/src/bagbag/Tools/Database/orator/seeds/seeder.py
+-rw-r--r--   0        0        0      203 2023-05-12 12:35:25.854288 bagbag-0.67.3/src/bagbag/Tools/Database/orator/seeds/stubs.py
+-rw-r--r--   0        0        0       60 2023-05-12 12:35:25.854476 bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-12 12:35:25.854566 bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/collection.py
+-rw-r--r--   0        0        0     2193 2023-05-12 12:35:25.854656 bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/fluent.py
+-rw-r--r--   0        0        0     2614 2023-05-12 12:35:25.854751 bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/grammar.py
+-rw-r--r--   0        0        0     2833 2023-05-12 12:35:25.855426 bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/__init__.py
+-rw-r--r--   0        0        0     4398 2023-05-12 12:35:25.855517 bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/command_formatter.py
+-rw-r--r--   0        0        0      749 2023-05-12 12:35:25.855603 bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/helpers.py
+-rw-r--r--   0        0        0      714 2023-05-12 12:35:25.855706 bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/qmarker.py
+-rw-r--r--   0        0        0     7566 2023-05-12 12:35:25.855800 bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/url.py
+-rw-r--r--   0        0        0    33893 2023-10-18 14:56:35.779826 bagbag-0.67.3/src/bagbag/Tools/Database/src.py
+-rw-r--r--   0        0        0     5251 2023-09-22 09:26:44.680084 bagbag-0.67.3/src/bagbag/Tools/DistributedLock_src.py
+-rw-r--r--   0        0        0     6759 2024-02-24 09:29:11.920490 bagbag-0.67.3/src/bagbag/Tools/Elasticsearch_src.py
+-rw-r--r--   0        0        0     4313 2023-09-22 09:26:44.687329 bagbag-0.67.3/src/bagbag/Tools/Github_src.py
+-rw-r--r--   0        0        0     1452 2023-09-22 09:26:44.687245 bagbag-0.67.3/src/bagbag/Tools/JavaScript_src.py
+-rw-r--r--   0        0        0    11103 2024-01-26 06:39:30.192158 bagbag-0.67.3/src/bagbag/Tools/Kafka_src.py
+-rw-r--r--   0        0        0     2029 2023-09-22 09:26:44.633507 bagbag-0.67.3/src/bagbag/Tools/Lock_src.py
+-rw-r--r--   0        0        0     6635 2023-09-22 09:26:44.687412 bagbag-0.67.3/src/bagbag/Tools/MatrixBot_src.py
+-rw-r--r--   0        0        0     1510 2024-01-12 08:41:39.736400 bagbag-0.67.3/src/bagbag/Tools/Nslookup_src.py
+-rw-r--r--   0        0        0     2365 2023-09-22 09:26:44.673022 bagbag-0.67.3/src/bagbag/Tools/OCR_src.py
+-rw-r--r--   0        0        0     3607 2024-05-10 12:51:32.811252 bagbag-0.67.3/src/bagbag/Tools/OpenAI.py
+-rw-r--r--   0        0        0     3716 2024-01-14 07:33:09.943287 bagbag-0.67.3/src/bagbag/Tools/ProgressBar_src.py
+-rw-r--r--   0        0        0     1661 2023-09-22 09:26:44.687535 bagbag-0.67.3/src/bagbag/Tools/Prometheus/MetricServer.py
+-rw-r--r--   0        0        0     3518 2024-02-02 03:59:39.001962 bagbag-0.67.3/src/bagbag/Tools/Prometheus/PushGateway.py
+-rw-r--r--   0        0        0      177 2024-01-15 06:37:19.255853 bagbag-0.67.3/src/bagbag/Tools/Prometheus/Utils.py
+-rw-r--r--   0        0        0      157 2024-01-15 06:36:14.708912 bagbag-0.67.3/src/bagbag/Tools/Prometheus/__init__.py
+-rw-r--r--   0        0        0     4750 2024-02-20 03:07:14.267082 bagbag-0.67.3/src/bagbag/Tools/Prometheus/metrics.py
+-rw-r--r--   0        0        0     2608 2023-09-22 09:26:44.680110 bagbag-0.67.3/src/bagbag/Tools/Queue_src.py
+-rw-r--r--   0        0        0     2491 2023-09-22 09:26:44.687633 bagbag-0.67.3/src/bagbag/Tools/RSS/Feed_src.py
+-rw-r--r--   0        0        0      662 2023-09-22 09:26:44.687624 bagbag-0.67.3/src/bagbag/Tools/RSS/Opml_src.py
+-rw-r--r--   0        0        0      619 2023-08-23 16:03:38.456528 bagbag-0.67.3/src/bagbag/Tools/RSS/__init__.py
+-rw-r--r--   0        0        0     3689 2023-09-22 09:26:44.572324 bagbag-0.67.3/src/bagbag/Tools/Ratelimit_src.py
+-rw-r--r--   0        0        0    26542 2024-05-08 06:59:03.274855 bagbag-0.67.3/src/bagbag/Tools/Redis_src.py
+-rw-r--r--   0        0        0     7168 2024-01-22 04:19:19.682899 bagbag-0.67.3/src/bagbag/Tools/SMTP_src.py
+-rw-r--r--   0        0        0     5610 2023-09-22 09:26:44.672664 bagbag-0.67.3/src/bagbag/Tools/SSH_src.py
+-rw-r--r--   0        0        0    35116 2024-05-11 01:54:49.889048 bagbag-0.67.3/src/bagbag/Tools/Selenium.py
+-rw-r--r--   0        0        0    14132 2023-09-22 09:26:44.680059 bagbag-0.67.3/src/bagbag/Tools/TelegramAsync.py
+-rw-r--r--   0        0        0     5112 2023-09-22 09:26:44.697272 bagbag-0.67.3/src/bagbag/Tools/TelegramBotOfficial_src.py
+-rw-r--r--   0        0        0     3070 2023-09-22 09:26:44.687395 bagbag-0.67.3/src/bagbag/Tools/TelegramBot_src.py
+-rw-r--r--   0        0        0    25972 2023-11-15 06:42:20.918334 bagbag-0.67.3/src/bagbag/Tools/Telegram_src.py
+-rw-r--r--   0        0        0      142 2023-05-12 12:35:25.824483 bagbag-0.67.3/src/bagbag/Tools/Test.py
+-rw-r--r--   0        0        0     3330 2023-07-30 16:03:16.992060 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/Bayes.py
+-rw-r--r--   0        0        0     3360 2023-07-30 16:04:55.755050 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/LogisticRegression.py
+-rw-r--r--   0        0        0     4443 2023-07-30 16:01:37.360637 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/SVM.py
+-rw-r--r--   0        0        0       96 2023-07-30 15:32:40.319669 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/__init__.py
+-rw-r--r--   0        0        0     6529 2023-09-22 09:26:44.687816 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/base.py
+-rw-r--r--   0        0        0    24552 2023-07-30 08:53:13.297800 bagbag-0.67.3/src/bagbag/Tools/TextClassifier/vars.py
+-rw-r--r--   0        0        0     4817 2023-09-22 09:26:44.687451 bagbag-0.67.3/src/bagbag/Tools/Translater.py
+-rw-r--r--   0        0        0    14103 2023-06-19 07:22:24.505061 bagbag-0.67.3/src/bagbag/Tools/Twitter/Browser_src.py
+-rw-r--r--   0        0        0    12719 2023-09-22 09:26:44.697186 bagbag-0.67.3/src/bagbag/Tools/Twitter/Elevated_src.py
+-rw-r--r--   0        0        0     2094 2023-09-22 09:26:44.687644 bagbag-0.67.3/src/bagbag/Tools/Twitter/Essential_src.py
+-rw-r--r--   0        0        0    29455 2023-08-03 11:34:20.274523 bagbag-0.67.3/src/bagbag/Tools/Twitter/Nitter_src.py
+-rw-r--r--   0        0        0     2744 2023-06-16 08:15:42.223073 bagbag-0.67.3/src/bagbag/Tools/Twitter/Utils.py
+-rw-r--r--   0        0        0     1070 2023-07-19 12:53:41.487474 bagbag-0.67.3/src/bagbag/Tools/Twitter/__init__.py
+-rw-r--r--   0        0        0     3298 2023-09-22 09:26:44.672824 bagbag-0.67.3/src/bagbag/Tools/URL_src.py
+-rw-r--r--   0        0        0      768 2023-09-22 09:26:44.680096 bagbag-0.67.3/src/bagbag/Tools/WaitGroup_src.py
+-rw-r--r--   0        0        0     8127 2023-09-22 09:26:44.687287 bagbag-0.67.3/src/bagbag/Tools/WebCrawler_src.py
+-rw-r--r--   0        0        0     7210 2024-04-09 13:05:04.493796 bagbag-0.67.3/src/bagbag/Tools/WebServer_src.py
+-rw-r--r--   0        0        0     3467 2023-12-15 09:08:11.884051 bagbag-0.67.3/src/bagbag/Tools/XPath_src.py
+-rw-r--r--   0        0        0     3236 2023-09-22 09:26:44.572163 bagbag-0.67.3/src/bagbag/Tools/Xlsx.py
+-rw-r--r--   0        0        0     3773 2024-05-11 01:55:16.853439 bagbag-0.67.3/src/bagbag/Tools/__init__.py
+-rw-r--r--   0        0        0     9404 2023-09-07 06:44:18.178279 bagbag-0.67.3/src/bagbag/Tools/pygtrans/ApiKeyTranslate.py
+-rw-r--r--   0        0        0      664 2023-09-07 06:44:18.178362 bagbag-0.67.3/src/bagbag/Tools/pygtrans/DetectResponse.py
+-rw-r--r--   0        0        0      424 2023-09-07 06:44:18.178562 bagbag-0.67.3/src/bagbag/Tools/pygtrans/LanguageResponse.py
+-rw-r--r--   0        0        0      418 2023-09-07 06:44:18.178627 bagbag-0.67.3/src/bagbag/Tools/pygtrans/Null.py
+-rw-r--r--   0        0        0     8717 2023-09-07 06:45:37.193201 bagbag-0.67.3/src/bagbag/Tools/pygtrans/Translate.py
+-rw-r--r--   0        0        0     1238 2023-09-07 06:44:18.178758 bagbag-0.67.3/src/bagbag/Tools/pygtrans/TranslateResponse.py
+-rw-r--r--   0        0        0      710 2023-09-07 06:44:18.178865 bagbag-0.67.3/src/bagbag/Tools/pygtrans/__init__.py
+-rw-r--r--   0        0        0     4560 2023-10-18 11:53:05.137309 bagbag-0.67.3/src/bagbag/__init__.py
+-rw-r--r--   0        0        0    20049 1970-01-01 00:00:00.000000 bagbag-0.67.3/PKG-INFO
```

### Comparing `bagbag-0.67.2/LICENSE` & `bagbag-0.67.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/README.md` & `bagbag-0.67.3/README.md`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/pyproject.toml` & `bagbag-0.67.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bagbag"
-version = "0.67.2"
+version = "0.67.3"
 description = "An all in one python library"
 
 license = "MIT"
 
 authors = [
     "Darren"
 ]
```

### Comparing `bagbag-0.67.2/src/bagbag/Cmd/__init__.py` & `bagbag-0.67.3/src/bagbag/Cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Cmd/src.py` & `bagbag-0.67.3/src/bagbag/Cmd/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Cryptoo/src.py` & `bagbag-0.67.3/src/bagbag/Cryptoo/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/File/src.py` & `bagbag-0.67.3/src/bagbag/File/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/CutSentenceStopWords_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/CutSentenceStopWords_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/CutSentence_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/CutSentence_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/FakeIdentity_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/FakeIdentity_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/FileType_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/FileType_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/Format/src.py` & `bagbag-0.67.3/src/bagbag/Funcs/Format/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/GetPublicIP_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/GetPublicIP_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/Ping_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/Ping_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/ResizeImage_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/ResizeImage_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/Wget_src.py` & `bagbag-0.67.3/src/bagbag/Funcs/Wget_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/__init__.py` & `bagbag-0.67.3/src/bagbag/Funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/whois/__init__.py` & `bagbag-0.67.3/src/bagbag/Funcs/whois/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/whois/data/public_suffix_list.dat` & `bagbag-0.67.3/src/bagbag/Funcs/whois/data/public_suffix_list.dat`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/whois/parser.py` & `bagbag-0.67.3/src/bagbag/Funcs/whois/parser.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/whois/time_zones.py` & `bagbag-0.67.3/src/bagbag/Funcs/whois/time_zones.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Funcs/whois/whois.py` & `bagbag-0.67.3/src/bagbag/Funcs/whois/whois.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Hash/__init__.py` & `bagbag-0.67.3/src/bagbag/Hash/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Hash/src.py` & `bagbag-0.67.3/src/bagbag/Hash/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Http/__init__.py` & `bagbag-0.67.3/src/bagbag/Http/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Http/src.py` & `bagbag-0.67.3/src/bagbag/Http/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Json/src.py` & `bagbag-0.67.3/src/bagbag/Json/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Lg.py` & `bagbag-0.67.3/src/bagbag/Lg.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Math/src.py` & `bagbag-0.67.3/src/bagbag/Math/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Os/Path/__init__.py` & `bagbag-0.67.3/src/bagbag/Os/Path/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Os/Path/src.py` & `bagbag-0.67.3/src/bagbag/Os/Path/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Os/__init__.py` & `bagbag-0.67.3/src/bagbag/Os/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Os/src.py` & `bagbag-0.67.3/src/bagbag/Os/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Process/src.py` & `bagbag-0.67.3/src/bagbag/Process/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Python/src.py` & `bagbag-0.67.3/src/bagbag/Python/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Random/src.py` & `bagbag-0.67.3/src/bagbag/Random/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Socket/TCP/src.py` & `bagbag-0.67.3/src/bagbag/Socket/TCP/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Socket/UDP/src.py` & `bagbag-0.67.3/src/bagbag/Socket/UDP/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/String/src.py` & `bagbag-0.67.3/src/bagbag/String/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/String/tlds.txt` & `bagbag-0.67.3/src/bagbag/String/tlds.txt`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/String/vars.py` & `bagbag-0.67.3/src/bagbag/String/vars.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Thread/src.py` & `bagbag-0.67.3/src/bagbag/Thread/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Time/__init__.py` & `bagbag-0.67.3/src/bagbag/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Time/src.py` & `bagbag-0.67.3/src/bagbag/Time/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Argparser_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Argparser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py` & `bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/CoinsPrice_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py` & `bagbag-0.67.3/src/bagbag/Tools/BlockChain/Binance/OfficialAccountVertify/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/BlockChain/CoinMarketCap/api.py` & `bagbag-0.67.3/src/bagbag/Tools/BlockChain/CoinMarketCap/api.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/BlockChain/Others/FearAndGreedIndex_src.py` & `bagbag-0.67.3/src/bagbag/Tools/BlockChain/Others/FearAndGreedIndex_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/BlockChain/Tron/src.py` & `bagbag-0.67.3/src/bagbag/Tools/BlockChain/Tron/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/CSV.py` & `bagbag-0.67.3/src/bagbag/Tools/CSV.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Cache.py` & `bagbag-0.67.3/src/bagbag/Tools/Cache.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Chan_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Chan_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/ComputerVision.py` & `bagbag-0.67.3/src/bagbag/Tools/ComputerVision.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Crontab_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Crontab_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/application.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/application.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/install_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/migrate_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/refresh_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/reset_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/rollback_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/migrations/status_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/models/make_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/models/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/make_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/commands/seeds/seed_command.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/connection.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/connection_interface.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/connection_interface.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/mysql_connection.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/mysql_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/postgres_connection.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connections/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/connection_factory.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/connection_factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/connector.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/postgres_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/connectors/sqlite_connector.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/database_manager.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/database_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/abstract_asset.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/column.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/column.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/column_diff.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/column_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/comparator.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/comparator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/foreign_key_constraint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/index.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/index.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/mysql_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/postgresql_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/keywords/sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/mysql57_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/mysql_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/postgres_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/platforms/sqlite_platform.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/postgres_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/schema_manager.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/sqlite_schema_manager.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/table.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/table.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/dbal/table_diff.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/dbal/table_diff.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/events/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/events/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/connectors.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/connectors.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/exceptions/orm.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/exceptions/orm.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/database_migration_repository.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/migration_creator.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/migration_creator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/migrator.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/migrator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/migrations/stubs.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/migrations/stubs.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/builder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/collection.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/collection.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/factory.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/factory.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/factory_builder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/factory_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/mixins/soft_deletes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/model.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/model.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/belongs_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/belongs_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_many_through.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_one.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/has_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_one.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_one_or_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_to.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/morph_to_many.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/pivot.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/pivot.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/relation.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/relation.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/result.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/result.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/relations/wrapper.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/scopes/soft_deleting.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/orm/utils.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/orm/utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/base.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/length_aware_paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/pagination/paginator.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/builder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/join_clause.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/join_clause.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/mysql_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/postgres_processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/query/processors/processor.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/query/processors/processor.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/blueprint.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/blueprint.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/builder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/mysql_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/postgres_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/grammars/sqlite_grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/mysql_builder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/mysql_builder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/schema/schema.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/schema/schema.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/seeds/seeder.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/seeds/seeder.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/fluent.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/fluent.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/support/grammar.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/support/grammar.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/command_formatter.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/command_formatter.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/helpers.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/qmarker.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/qmarker.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/orator/utils/url.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/orator/utils/url.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Database/src.py` & `bagbag-0.67.3/src/bagbag/Tools/Database/src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/DistributedLock_src.py` & `bagbag-0.67.3/src/bagbag/Tools/DistributedLock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Elasticsearch_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Elasticsearch_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Github_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Github_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/JavaScript_src.py` & `bagbag-0.67.3/src/bagbag/Tools/JavaScript_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Kafka_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Kafka_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Lock_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Lock_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/MatrixBot_src.py` & `bagbag-0.67.3/src/bagbag/Tools/MatrixBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Nslookup_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Nslookup_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/OCR_src.py` & `bagbag-0.67.3/src/bagbag/Tools/OCR_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/OpenAI.py` & `bagbag-0.67.3/src/bagbag/Tools/OpenAI.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/ProgressBar_src.py` & `bagbag-0.67.3/src/bagbag/Tools/ProgressBar_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Prometheus/MetricServer.py` & `bagbag-0.67.3/src/bagbag/Tools/Prometheus/MetricServer.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Prometheus/PushGateway.py` & `bagbag-0.67.3/src/bagbag/Tools/Prometheus/PushGateway.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Prometheus/metrics.py` & `bagbag-0.67.3/src/bagbag/Tools/Prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Queue_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Queue_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/RSS/Feed_src.py` & `bagbag-0.67.3/src/bagbag/Tools/RSS/Feed_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/RSS/Opml_src.py` & `bagbag-0.67.3/src/bagbag/Tools/RSS/Opml_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/RSS/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/RSS/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Ratelimit_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Ratelimit_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Redis_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Redis_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/SMTP_src.py` & `bagbag-0.67.3/src/bagbag/Tools/SMTP_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/SSH_src.py` & `bagbag-0.67.3/src/bagbag/Tools/SSH_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Selenium.py` & `bagbag-0.67.3/src/bagbag/Tools/Selenium.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,33 +179,33 @@
 
         elif self.browserName == "firefox":
             res = func(self, *args, **kwargs)
             return 
 
     return ware
 
-# > The seleniumElement class is a wrapper for the selenium.webdriver.remote.webelement.WebElement
+# > The SeleniumElement class is a wrapper for the selenium.webdriver.remote.webelement.WebElement
 # class
-class seleniumElement():
+class SeleniumElement():
     def __init__(self, element:selenium.webdriver.remote.webelement.WebElement, se:seleniumBase):
         self.element = element
         self.se = se
         self.driver = self.se.driver
         self.browserName = self.se.browserName
         self.browserRemote = self.se.browserRemote
     
-    def Clear(self) -> seleniumElement:
+    def Clear(self) -> SeleniumElement:
         """
         Clear() clears the text if it's a text entry element
         """
         self.element.clear()
         return self
     
     @retryOnError
-    def Click(self) -> seleniumElement:
+    def Click(self) -> SeleniumElement:
         """
         Click() is a function that clicks on an element
         """
         if self.browserName in ["chrome", "chromewire"] and not self.browserName:
             self.driver.execute_cdp_cmd('Network.setUserAgentOverride', {"userAgent": random.choice(useragents)['user_agent']})
 
         self.element.click()
@@ -225,58 +225,58 @@
         
         :param name: The name of the element
         :type name: str
         :return: The attribute of the element.
         """
         return self.element.get_attribute(name)
     
-    def Input(self, string:str) -> seleniumElement:
+    def Input(self, string:str) -> SeleniumElement:
         """
         The function Input() takes in a string and sends it to the element
         
         :param string: The string you want to input into the text box
         :type string: str
         """
         self.element.send_keys(string)
         return self
     
     @retryOnError
-    def Submit(self) -> seleniumElement:
+    def Submit(self) -> SeleniumElement:
         """
         Submit() is a function that submits the form that the element belongs to
         """
         if self.browserName in ["chrome", "chromewire"] and not self.browserName:
             self.driver.execute_cdp_cmd('Network.setUserAgentOverride', {"userAgent": random.choice(useragents)['user_agent']})
         
         self.element.submit()
 
         return self
     
     @retryOnError
-    def PressEnter(self) -> seleniumElement:
+    def PressEnter(self) -> SeleniumElement:
         """
         It takes the element that you want to press enter on and sends the enter key to it
         """
 
         if self.browserName  in ["chrome", "chromewire"] and not self.browserName:
             self.driver.execute_cdp_cmd('Network.setUserAgentOverride', {"userAgent": random.choice(useragents)['user_agent']})
         
         self.element.send_keys(webkeys.ENTER)
 
         return self
     
-    def ScrollIntoElement(self) -> seleniumElement:
+    def ScrollIntoElement(self) -> SeleniumElement:
         self.driver.execute_script("arguments[0].scrollIntoView(true);", self.element)
         return self
 
     def HTML(self) -> str:
         return self.element.get_attribute('innerHTML')
 
 class seleniumBase():
-    def Find(self, xpath:str|list, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> seleniumElement|None:
+    def Find(self, xpath:str|list, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> SeleniumElement|None:
         """
         This is a Python function that finds a Selenium element based on an XPath string or list of XPath
         strings, with optional parameters for timeout, scrolling, and retrying on errors.
         
         :param xpath: The xpath expression used to locate the element(s) on the webpage
         :type xpath: str|list
         :param timeout: The maximum amount of time (in seconds) to wait for the element to be found before
@@ -287,47 +287,47 @@
         specified XPath. If set to True, the page will be scrolled to bring the element into view before
         attempting to find it. If set to False, the, defaults to True
         :type scrollIntoElement: bool (optional)
         :param retryOnError: The retryOnError parameter specifies the number of times the function should
         retry finding the element if an error occurs during the search. If the element is not found after
         the specified number of retries, the function will return None, defaults to 5
         :type retryOnError: int (optional)
-        :return: The function `Find` returns a `seleniumElement` object if it is found, or `None` if it is
+        :return: The function `Find` returns a `SeleniumElement` object if it is found, or `None` if it is
         not found.
         """
         if type(xpath) == str:
             return self._find(xpath, timeout, scrollIntoElement, retryOnError)
         else:
             idx = self.Except(xpath, timeout=timeout)
             if idx == None:
                 return None 
             else:
                 return self._find(xpath[idx], timeout, scrollIntoElement, retryOnError)
 
-    def _find(self, xpath:str, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> seleniumElement|None:
+    def _find(self, xpath:str, timeout:int=60, scrollIntoElement:bool=True, retryOnError:int=5) -> SeleniumElement|None:
         """
         > Finds an element by xpath, waits for it to appear, and returns it
         
         :param xpath: The xpath of the element you want to find
         :type xpath: str
         :param timeout: , defaults to 8 second
         :type timeout: int (optional)
         :param scrollIntoElement: If True, the element will be scrolled into view before returning it,
         defaults to True
         :type scrollIntoElement: bool (optional)
-        :return: seleniumElement
+        :return: SeleniumElement
         """
         waited = 0
         errcount = 0
         while True:
             try:
                 el = self.driver.find_element(webby.XPATH, xpath)
                 if scrollIntoElement:
                     self.driver.execute_script("arguments[0].scrollIntoView(true);", el)
-                return seleniumElement(el, self)
+                return SeleniumElement(el, self)
             except selenium.common.exceptions.NoSuchElementException as e: 
                 if timeout == 0:
                     return None 
                 elif timeout == -1:
                     time.sleep(1)
                 elif timeout > 0:
                     time.sleep(1)
```

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TelegramAsync.py` & `bagbag-0.67.3/src/bagbag/Tools/TelegramAsync.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TelegramBotOfficial_src.py` & `bagbag-0.67.3/src/bagbag/Tools/TelegramBotOfficial_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TelegramBot_src.py` & `bagbag-0.67.3/src/bagbag/Tools/TelegramBot_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Telegram_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Telegram_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TextClassifier/Bayes.py` & `bagbag-0.67.3/src/bagbag/Tools/TextClassifier/Bayes.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TextClassifier/LogisticRegression.py` & `bagbag-0.67.3/src/bagbag/Tools/TextClassifier/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TextClassifier/SVM.py` & `bagbag-0.67.3/src/bagbag/Tools/TextClassifier/SVM.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TextClassifier/base.py` & `bagbag-0.67.3/src/bagbag/Tools/TextClassifier/base.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/TextClassifier/vars.py` & `bagbag-0.67.3/src/bagbag/Tools/TextClassifier/vars.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Translater.py` & `bagbag-0.67.3/src/bagbag/Tools/Translater.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/Browser_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/Browser_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/Elevated_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/Elevated_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/Essential_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/Essential_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/Nitter_src.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/Nitter_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/Utils.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/Utils.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Twitter/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/Twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/URL_src.py` & `bagbag-0.67.3/src/bagbag/Tools/URL_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/WaitGroup_src.py` & `bagbag-0.67.3/src/bagbag/Tools/WaitGroup_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/WebCrawler_src.py` & `bagbag-0.67.3/src/bagbag/Tools/WebCrawler_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/WebServer_src.py` & `bagbag-0.67.3/src/bagbag/Tools/WebServer_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/XPath_src.py` & `bagbag-0.67.3/src/bagbag/Tools/XPath_src.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/Xlsx.py` & `bagbag-0.67.3/src/bagbag/Tools/Xlsx.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     "BlockChain": ["BlockChain"], 
     "JavaScript": ["JavaScript"],
     # from . import ComputerVision
     "ComputerVision": ["ComputerVision"],
     "WebCrawler_src": ["WebCrawler"],
     "OCR_src": ["OCR"],
     # "File_src": ["File"],
-    "Selenium": ["Selenium", "SeleniumFlow"],
+    "Selenium": ["Selenium", "SeleniumFlow", "SeleniumElement"],
     "CSV": ["CSV"],
     "OpenAI": ["OpenAI"],
     "Prometheus": ['Prometheus'],
     "Cache": ["Cache"],
     "TextClassifier": ["TextClassifier"],
     "SMTP_src": ['SMTP']
 }
```

### Comparing `bagbag-0.67.2/src/bagbag/Tools/pygtrans/ApiKeyTranslate.py` & `bagbag-0.67.3/src/bagbag/Tools/pygtrans/ApiKeyTranslate.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/pygtrans/DetectResponse.py` & `bagbag-0.67.3/src/bagbag/Tools/pygtrans/DetectResponse.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/pygtrans/Translate.py` & `bagbag-0.67.3/src/bagbag/Tools/pygtrans/Translate.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/pygtrans/TranslateResponse.py` & `bagbag-0.67.3/src/bagbag/Tools/pygtrans/TranslateResponse.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/Tools/pygtrans/__init__.py` & `bagbag-0.67.3/src/bagbag/Tools/pygtrans/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/src/bagbag/__init__.py` & `bagbag-0.67.3/src/bagbag/__init__.py`

 * *Files identical despite different names*

### Comparing `bagbag-0.67.2/PKG-INFO` & `bagbag-0.67.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagbag
-Version: 0.67.2
+Version: 0.67.3
 Summary: An all in one python library
 Home-page: https://github.com/darren2046/bagbag
 License: MIT
 Keywords: base,library
 Author: Darren
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
```

