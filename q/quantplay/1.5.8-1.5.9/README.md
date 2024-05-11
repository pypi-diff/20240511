# Comparing `tmp/quantplay-1.5.8.tar.gz` & `tmp/quantplay-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.5.8.tar", last modified: Fri Mar 15 03:10:28 2024, max compression
+gzip compressed data, was "quantplay-1.5.9.tar", last modified: Fri Mar 15 04:41:41 2024, max compression
```

## Comparing `quantplay-1.5.8.tar` & `quantplay-1.5.9.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.403269 quantplay-1.5.8/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 03:10:28.403353 quantplay-1.5.8/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.5.8/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.382424 quantplay-1.5.8/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.383551 quantplay-1.5.8/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17974 2024-01-30 12:40:34.000000 quantplay-1.5.8/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.388326 quantplay-1.5.8/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    14854 2024-03-12 09:33:38.000000 quantplay-1.5.8/quantplay/broker/aliceblue.py
--rw-r--r--   0 ashok      (502) staff       (20)    16155 2024-03-12 13:50:49.000000 quantplay-1.5.8/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.388667 quantplay-1.5.8/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:38.000000 quantplay-1.5.8/quantplay/broker/finvasia_utils/fa_noren.py
--rw-r--r--   0 ashok      (502) staff       (20)     2717 2024-03-06 12:51:21.000000 quantplay-1.5.8/quantplay/broker/flattrade.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.389408 quantplay-1.5.8/quantplay/broker/ft_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-06 12:37:31.000000 quantplay-1.5.8/quantplay/broker/ft_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2247 2024-01-23 17:16:24.000000 quantplay-1.5.8/quantplay/broker/ft_utils/flattrade_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:42.000000 quantplay-1.5.8/quantplay/broker/ft_utils/ft_noren.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.389886 quantplay-1.5.8/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    42895 2024-03-12 06:29:22.000000 quantplay-1.5.8/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.5.8/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      750 2024-03-14 07:46:45.000000 quantplay-1.5.8/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     3862 2024-03-09 04:22:31.000000 quantplay-1.5.8/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    26560 2024-03-12 09:32:00.000000 quantplay-1.5.8/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    17924 2024-03-13 04:41:41.000000 quantplay-1.5.8/quantplay/broker/noren.py
--rw-r--r--   0 ashok      (502) staff       (20)     2515 2024-03-06 12:50:44.000000 quantplay-1.5.8/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.5.8/quantplay/broker/symphony.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.390455 quantplay-1.5.8/quantplay/broker/uplink/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-10 17:08:05.000000 quantplay-1.5.8/quantplay/broker/uplink/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     4019 2024-03-11 14:33:40.000000 quantplay-1.5.8/quantplay/broker/uplink/uplink_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    15325 2024-03-14 04:29:38.000000 quantplay-1.5.8/quantplay/broker/upstox.py
--rw-r--r--   0 ashok      (502) staff       (20)    21807 2024-03-15 03:09:59.000000 quantplay-1.5.8/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.391842 quantplay-1.5.8/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33459 2024-03-15 03:09:39.000000 quantplay-1.5.8/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     2900 2024-01-10 08:54:27.000000 quantplay-1.5.8/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6422 2024-01-10 08:54:27.000000 quantplay-1.5.8/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9365 2024-02-29 11:34:06.000000 quantplay-1.5.8/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    15190 2024-03-14 05:10:02.000000 quantplay-1.5.8/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.391938 quantplay-1.5.8/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.392143 quantplay-1.5.8/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-08-08 03:19:52.000000 quantplay-1.5.8/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.392530 quantplay-1.5.8/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28456 2023-08-22 08:10:22.000000 quantplay-1.5.8/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.393272 quantplay-1.5.8/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    18224 2023-09-25 04:30:48.000000 quantplay-1.5.8/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.393477 quantplay-1.5.8/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.5.8/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.5.8/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.393818 quantplay-1.5.8/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     3040 2024-03-03 06:58:26.000000 quantplay-1.5.8/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.394192 quantplay-1.5.8/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.394692 quantplay-1.5.8/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.394917 quantplay-1.5.8/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.395548 quantplay-1.5.8/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.5.8/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.395811 quantplay-1.5.8/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.395973 quantplay-1.5.8/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.396200 quantplay-1.5.8/quantplay/options/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-12-24 05:33:30.000000 quantplay-1.5.8/quantplay/options/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1964 2024-02-03 08:46:26.000000 quantplay-1.5.8/quantplay/options/analytics.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.396674 quantplay-1.5.8/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.397133 quantplay-1.5.8/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.5.8/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.5.8/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.5.8/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.397803 quantplay-1.5.8/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.5.8/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.5.8/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398116 quantplay-1.5.8/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.5.8/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398206 quantplay-1.5.8/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.5.8/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398302 quantplay-1.5.8/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.5.8/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398395 quantplay-1.5.8/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.5.8/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398508 quantplay-1.5.8/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.5.8/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398619 quantplay-1.5.8/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.5.8/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.398741 quantplay-1.5.8/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.5.8/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.399435 quantplay-1.5.8/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.5.8/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.5.8/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.5.8/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.5.8/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.399947 quantplay-1.5.8/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.5.8/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:05.000000 quantplay-1.5.8/quantplay/strategy/investment_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:44.000000 quantplay-1.5.8/quantplay/strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.5.8/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.401491 quantplay-1.5.8/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.5.8/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5446 2023-10-07 15:49:03.000000 quantplay-1.5.8/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1664 2024-01-16 16:34:52.000000 quantplay-1.5.8/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1225 2023-10-08 10:27:32.000000 quantplay-1.5.8/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.5.8/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.401634 quantplay-1.5.8/quantplay/wrapper/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:53:58.000000 quantplay-1.5.8/quantplay/wrapper/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.401860 quantplay-1.5.8/quantplay/wrapper/aws/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:54:05.000000 quantplay-1.5.8/quantplay/wrapper/aws/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1157 2023-09-06 14:08:43.000000 quantplay-1.5.8/quantplay/wrapper/aws/s3.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.383345 quantplay-1.5.8/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 03:10:28.000000 quantplay-1.5.8/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3922 2024-03-15 03:10:28.000000 quantplay-1.5.8/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2024-03-15 03:10:28.000000 quantplay-1.5.8/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      321 2024-03-15 03:10:28.000000 quantplay-1.5.8/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2024-03-15 03:10:28.000000 quantplay-1.5.8/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2024-03-15 03:10:28.403565 quantplay-1.5.8/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      875 2024-03-15 03:10:23.000000 quantplay-1.5.8/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.402095 quantplay-1.5.8/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.5.8/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.402415 quantplay-1.5.8/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/broker/finvasia.py
--rw-r--r--   0 ashok      (502) staff       (20)     1228 2023-10-06 09:00:31.000000 quantplay-1.5.8/test/broker/motilal.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.402748 quantplay-1.5.8/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 03:10:28.403124 quantplay-1.5.8/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.5.8/test/strategy/sample_strategy.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807682 quantplay-1.5.9/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 04:41:41.807766 quantplay-1.5.9/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.5.9/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.786357 quantplay-1.5.9/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.787330 quantplay-1.5.9/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17974 2024-01-30 12:40:34.000000 quantplay-1.5.9/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.791943 quantplay-1.5.9/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    14854 2024-03-12 09:33:38.000000 quantplay-1.5.9/quantplay/broker/aliceblue.py
+-rw-r--r--   0 ashok      (502) staff       (20)    16155 2024-03-12 13:50:49.000000 quantplay-1.5.9/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.792326 quantplay-1.5.9/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:38.000000 quantplay-1.5.9/quantplay/broker/finvasia_utils/fa_noren.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2717 2024-03-06 12:51:21.000000 quantplay-1.5.9/quantplay/broker/flattrade.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.793109 quantplay-1.5.9/quantplay/broker/ft_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-06 12:37:31.000000 quantplay-1.5.9/quantplay/broker/ft_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2247 2024-01-23 17:16:24.000000 quantplay-1.5.9/quantplay/broker/ft_utils/flattrade_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    32131 2024-03-14 05:08:42.000000 quantplay-1.5.9/quantplay/broker/ft_utils/ft_noren.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.793612 quantplay-1.5.9/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    43058 2024-03-15 04:40:14.000000 quantplay-1.5.9/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.5.9/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      750 2024-03-14 07:46:45.000000 quantplay-1.5.9/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3862 2024-03-09 04:22:31.000000 quantplay-1.5.9/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    26560 2024-03-12 09:32:00.000000 quantplay-1.5.9/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17924 2024-03-13 04:41:41.000000 quantplay-1.5.9/quantplay/broker/noren.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2515 2024-03-06 12:50:44.000000 quantplay-1.5.9/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/broker/symphony.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.794149 quantplay-1.5.9/quantplay/broker/uplink/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-10 17:08:05.000000 quantplay-1.5.9/quantplay/broker/uplink/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4019 2024-03-11 14:33:40.000000 quantplay-1.5.9/quantplay/broker/uplink/uplink_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    15325 2024-03-14 04:29:38.000000 quantplay-1.5.9/quantplay/broker/upstox.py
+-rw-r--r--   0 ashok      (502) staff       (20)    21807 2024-03-15 03:09:59.000000 quantplay-1.5.9/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.795681 quantplay-1.5.9/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33459 2024-03-15 03:09:39.000000 quantplay-1.5.9/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2900 2024-01-10 08:54:27.000000 quantplay-1.5.9/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6422 2024-01-10 08:54:27.000000 quantplay-1.5.9/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9365 2024-02-29 11:34:06.000000 quantplay-1.5.9/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    15190 2024-03-14 05:10:02.000000 quantplay-1.5.9/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.795873 quantplay-1.5.9/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.796118 quantplay-1.5.9/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-08-08 03:19:52.000000 quantplay-1.5.9/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.796582 quantplay-1.5.9/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28456 2023-08-22 08:10:22.000000 quantplay-1.5.9/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797429 quantplay-1.5.9/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    18224 2023-09-25 04:30:48.000000 quantplay-1.5.9/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797605 quantplay-1.5.9/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-06-23 06:49:50.000000 quantplay-1.5.9/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.797884 quantplay-1.5.9/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3040 2024-03-03 06:58:26.000000 quantplay-1.5.9/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798211 quantplay-1.5.9/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798665 quantplay-1.5.9/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.798902 quantplay-1.5.9/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799515 quantplay-1.5.9/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.5.9/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799804 quantplay-1.5.9/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.799973 quantplay-1.5.9/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.800165 quantplay-1.5.9/quantplay/options/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-12-24 05:33:30.000000 quantplay-1.5.9/quantplay/options/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1964 2024-02-03 08:46:26.000000 quantplay-1.5.9/quantplay/options/analytics.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.800650 quantplay-1.5.9/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.801145 quantplay-1.5.9/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10801 2023-06-23 06:49:43.000000 quantplay-1.5.9/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.5.9/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.5.9/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802117 quantplay-1.5.9/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.5.9/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11648 2023-06-23 06:49:43.000000 quantplay-1.5.9/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802361 quantplay-1.5.9/quantplay/strategies/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802476 quantplay-1.5.9/quantplay/strategies/equities/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802591 quantplay-1.5.9/quantplay/strategies/equities/intraday/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802696 quantplay-1.5.9/quantplay/strategies/equities/overnight/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802795 quantplay-1.5.9/quantplay/strategies/futures/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.802893 quantplay-1.5.9/quantplay/strategies/futures/overnight/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.803006 quantplay-1.5.9/quantplay/strategies/options/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.803645 quantplay-1.5.9/quantplay/strategies/options/intraday/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2024-03-15 03:15:32.000000 quantplay-1.5.9/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.804154 quantplay-1.5.9/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.5.9/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:05.000000 quantplay-1.5.9/quantplay/strategy/investment_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-21 06:34:44.000000 quantplay-1.5.9/quantplay/strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.5.9/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.805833 quantplay-1.5.9/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.5.9/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5446 2023-10-07 15:49:03.000000 quantplay-1.5.9/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1664 2024-01-16 16:34:52.000000 quantplay-1.5.9/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1225 2023-10-08 10:27:32.000000 quantplay-1.5.9/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.5.9/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.805971 quantplay-1.5.9/quantplay/wrapper/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:53:58.000000 quantplay-1.5.9/quantplay/wrapper/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806184 quantplay-1.5.9/quantplay/wrapper/aws/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-09-06 13:54:05.000000 quantplay-1.5.9/quantplay/wrapper/aws/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1157 2023-09-06 14:08:43.000000 quantplay-1.5.9/quantplay/wrapper/aws/s3.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.787118 quantplay-1.5.9/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      662 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3922 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      321 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2024-03-15 04:41:41.000000 quantplay-1.5.9/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2024-03-15 04:41:41.808027 quantplay-1.5.9/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      875 2024-03-15 04:41:38.000000 quantplay-1.5.9/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806432 quantplay-1.5.9/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.5.9/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.806751 quantplay-1.5.9/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/broker/finvasia.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1228 2023-10-06 09:00:31.000000 quantplay-1.5.9/test/broker/motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807111 quantplay-1.5.9/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2024-03-15 04:41:41.807492 quantplay-1.5.9/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.5.9/test/strategy/sample_strategy.py
```

### Comparing `quantplay-1.5.8/PKG-INFO` & `quantplay-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.5.8
+Version: 1.5.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.5.8/quantplay/backtest/backtest_trades.py` & `quantplay-1.5.9/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/aliceblue.py` & `quantplay-1.5.9/quantplay/broker/aliceblue.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/angelone.py` & `quantplay-1.5.9/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/broker_client.py` & `quantplay-1.5.9/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/finvasia_utils/fa_noren.py` & `quantplay-1.5.9/quantplay/broker/finvasia_utils/fa_noren.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/flattrade.py` & `quantplay-1.5.9/quantplay/broker/flattrade.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/ft_utils/flattrade_utils.py` & `quantplay-1.5.9/quantplay/broker/ft_utils/flattrade_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/ft_utils/ft_noren.py` & `quantplay-1.5.9/quantplay/broker/ft_utils/ft_noren.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/generics/broker.py` & `quantplay-1.5.9/quantplay/broker/generics/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,14 +608,15 @@
             open_orders = open_orders[open_orders.tradingsymbol.isin(tradingsymbols)]
 
         order_ids = open_orders.order_id.to_list()
         for order_id in order_ids:
             self.cancel_order(order_id)
             time.sleep(0.1)
 
+    @timeit(MetricName="Broker:square_off_all")
     def square_off_all(
         self,
         dry_run=True,
         contains=None,
         option_type=None,
         sleep_time=0.1,
         keep_hedges=False,
@@ -1111,16 +1112,20 @@
 
         return self.place_large_orders(orders)
 
     def modify_orders_till_complete(
         self, orders_placed, sleep_time=10, max_modification_count=10
     ):
         modification_count = {}
+        skip_first_sleep = True
         while 1:
-            time.sleep(sleep_time)
+            if not skip_first_sleep:
+                time.sleep(sleep_time)
+                skip_first_sleep = False
+
             orders = self.orders()
 
             orders = orders[orders.order_id.isin(orders_placed)]
             orders = orders[~orders.status.isin(["REJECTED", "CANCELLED", "COMPLETE"])]
 
             if len(orders) == 0:
                 Constants.logger.info("ALL orders have been completed")
```

### Comparing `quantplay-1.5.8/quantplay/broker/iifl.py` & `quantplay-1.5.9/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/iifl_xts.py` & `quantplay-1.5.9/quantplay/broker/iifl_xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/kite_utils.py` & `quantplay-1.5.9/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/motilal.py` & `quantplay-1.5.9/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/noren.py` & `quantplay-1.5.9/quantplay/broker/noren.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/shoonya.py` & `quantplay-1.5.9/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/symphony.py` & `quantplay-1.5.9/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/uplink/uplink_utils.py` & `quantplay-1.5.9/quantplay/broker/uplink/uplink_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/upstox.py` & `quantplay-1.5.9/quantplay/broker/upstox.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/xts.py` & `quantplay-1.5.9/quantplay/broker/xts.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.5.9/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/broker/zerodha.py` & `quantplay-1.5.9/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.5.9/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/brokerage/generics/broker.py` & `quantplay-1.5.9/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.5.9/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/config/qplay_config.py` & `quantplay-1.5.9/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/create_sample_data.py` & `quantplay-1.5.9/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/data_modify_script.py` & `quantplay-1.5.9/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/date_fix.py` & `quantplay-1.5.9/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/exception/exceptions.py` & `quantplay-1.5.9/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/executor/strategy_executor.py` & `quantplay-1.5.9/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/indicators/Indicator.py` & `quantplay-1.5.9/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/model/exchange/instrument.py` & `quantplay-1.5.9/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/model/exchange/order.py` & `quantplay-1.5.9/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/model/exchange/tick.py` & `quantplay-1.5.9/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/options/analytics.py` & `quantplay-1.5.9/quantplay/options/analytics.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.5.9/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/order_execution/mean_price.py` & `quantplay-1.5.9/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/reporting/strategy_report.py` & `quantplay-1.5.9/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/reporting/visuals.py` & `quantplay-1.5.9/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/services/market.py` & `quantplay-1.5.9/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/services/tradelens.py` & `quantplay-1.5.9/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.5.9/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.5.9/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/strategy/base.py` & `quantplay-1.5.9/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/config_util.py` & `quantplay-1.5.9/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/constant.py` & `quantplay-1.5.9/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/data_utils.py` & `quantplay-1.5.9/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/exchange.py` & `quantplay-1.5.9/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/number_utils.py` & `quantplay-1.5.9/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/pickle_utils.py` & `quantplay-1.5.9/quantplay/utils/pickle_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/selenium_utils.py` & `quantplay-1.5.9/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/utils/transaction_utils.py` & `quantplay-1.5.9/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay/wrapper/aws/s3.py` & `quantplay-1.5.9/quantplay/wrapper/aws/s3.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/quantplay.egg-info/PKG-INFO` & `quantplay-1.5.9/quantplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.5.8
+Version: 1.5.9
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.5.8/quantplay.egg-info/SOURCES.txt` & `quantplay-1.5.9/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/setup.py` & `quantplay-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.5.8",
+    version="1.5.9",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.5.8/test/broker/motilal.py` & `quantplay-1.5.9/test/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.5.8/test/strategy/sample_strategy.py` & `quantplay-1.5.9/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

