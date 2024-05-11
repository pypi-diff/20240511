# Comparing `tmp/openbb_nightly-4.1.7.dev202405090009.tar.gz` & `tmp/openbb_nightly-4.1.7.dev202405100010.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nightly-4.1.7.dev202405090009.tar", max compression
+gzip compressed data, was "openbb_nightly-4.1.7.dev202405100010.tar", max compression
```

## Comparing `openbb_nightly-4.1.7.dev202405090009.tar` & `openbb_nightly-4.1.7.dev202405100010.tar`

### file list

```diff
@@ -1,791 +1,791 @@
--rw-r--r--   0        0        0     6818 2024-05-09 00:09:48.243605 openbb_nightly-4.1.7.dev202405090009/README.md
--rw-r--r--   0        0        0       19 2024-05-09 00:09:48.243605 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-05-09 00:09:48.243605 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    18672 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1908 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/api_settings.py
--rw-r--r--   0        0        0     1035 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3875 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      502 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2233 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1054 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/field.py
--rw-r--r--   0        0        0      694 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9094 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1477 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0      801 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/python_settings.py
--rw-r--r--   0        0        0       37 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     4044 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21268 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10402 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3511 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    65939 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2224 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-05-09 00:09:48.247606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1368 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2581 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8142 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0     1377 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/available_indicators.py
--rw-r--r--   0        0        0      630 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1246 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     3722 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/country_profile.py
--rw-r--r--   0        0        0     1591 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      423 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2377 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1680 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/economic_indicators.py
--rw-r--r--   0        0        0     1750 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      912 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1445 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      902 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     2390 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-05-09 00:09:48.251606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3073 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3526 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9699 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.255606 openbb_nightly-4.1.7.dev202405090009/core/openbb_core/py.typed
--rw-r--r--   0        0        0       34 2024-05-09 00:09:48.259606 openbb_nightly-4.1.7.dev202405090009/extensions/commodity/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-05-09 00:09:48.259606 openbb_nightly-4.1.7.dev202405090009/extensions/commodity/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0       31 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/py.typed
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/__init__.py
--rw-r--r--   0        0        0     3848 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/currency_router.py
--rw-r--r--   0        0        0       38 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/price/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/py.typed
--rw-r--r--   0        0        0       15 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0       39 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/devtools/openbb_devtools/__init__.py
--rw-r--r--   0        0        0       37 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-05-09 00:09:48.263605 openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/utils.py
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/__init__.py
--rw-r--r--   0        0        0    12007 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/py.typed
--rw-r--r--   0        0        0       19 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     3832 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/py.typed
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.267605 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0       23 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/py.typed
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/news/openbb_news/__init__.py
--rw-r--r--   0        0        0     3213 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/news/openbb_news/news_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/news/openbb_news/py.typed
--rw-r--r--   0        0        0       59 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0       35 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-05-09 00:09:48.271606 openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0       43 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    63911 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/technical_router.py
--rw-r--r--   0        0        0    21550 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/__init__.py
--rw-r--r--   0        0        0     1852 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/builder.py
--rw-r--r--   0        0        0    40926 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/charting_router.py
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/__init__.py
--rw-r--r--   0        0        0   418780 2024-05-09 00:09:48.275606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
--rw-r--r--   0        0        0  3585992 2024-05-09 00:09:48.291605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
--rw-r--r--   0        0        0    17442 2024-05-09 00:09:48.291605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/backend.py
--rw-r--r--   0        0        0     7362 2024-05-09 00:09:48.291605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/chart_style.py
--rw-r--r--   0        0        0       42 2024-05-09 00:09:48.295606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/config/__init__.py
--rw-r--r--   0        0        0     8068 2024-05-09 00:09:48.295606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
--rw-r--r--   0        0        0     2554 2024-05-09 00:09:48.295606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
--rw-r--r--   0        0        0    58532 2024-05-09 00:09:48.295606 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
--rw-r--r--   0        0        0  5228579 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly.html
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
--rw-r--r--   0        0        0     7185 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
--rw-r--r--   0        0        0    12381 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
--rw-r--r--   0        0        0       25 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
--rw-r--r--   0        0        0     8555 2024-05-09 00:09:48.315605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
--rw-r--r--   0        0        0    19572 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
--rw-r--r--   0        0        0     3300 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
--rw-r--r--   0        0        0     5697 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
--rw-r--r--   0        0        0     6877 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
--rw-r--r--   0        0        0     3547 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
--rw-r--r--   0        0        0    25006 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
--rw-r--r--   0        0        0     1437 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
--rw-r--r--   0        0        0   717892 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/table.html
--rw-r--r--   0        0        0     2246 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/to_chart.py
--rw-r--r--   0        0        0    26843 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/query_params.py
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/__init__.py
--rw-r--r--   0        0        0      603 2024-05-09 00:09:48.319605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/colors.py
--rw-r--r--   0        0        0     3462 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
--rw-r--r--   0        0        0     3491 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
--rw-r--r--   0        0        0     2505 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/__init__.py
--rw-r--r--   0        0        0    20295 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
--rw-r--r--   0        0        0     2493 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/helpers.py
--rw-r--r--   0        0        0    16657 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
--rw-r--r--   0        0        0     1440 2024-05-09 00:09:48.323605 openbb_nightly-4.1.7.dev202405090009/openbb/__init__.py
--rw-r--r--   0        0        0  1227796 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/assets/reference.json
--rw-r--r--   0        0        0     2813 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/__extensions__.py
--rw-r--r--   0        0        0     3299 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/crypto.py
--rw-r--r--   0        0        0     6468 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    13823 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/currency.py
--rw-r--r--   0        0        0     6360 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/derivatives.py
--rw-r--r--   0        0        0    12047 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    65869 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/economy.py
--rw-r--r--   0        0        0    12355 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27558 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity.py
--rw-r--r--   0        0        0    18353 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2807 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    25823 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    40717 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   163990 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30431 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26606 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3710 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    75407 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/etf.py
--rw-r--r--   0        0        0     4538 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19470 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     7001 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    26229 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    10857 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11744 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/index.py
--rw-r--r--   0        0        0    20588 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/package/regulators.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/openbb/py.typed
--rw-r--r--   0        0        0     1106 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12452 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5288 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-05-09 00:09:48.327605 openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      877 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    18079 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6173 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9801 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      779 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-05-09 00:09:48.331605 openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0     1779 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8338 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9657 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8336 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4831 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     7796 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-05-09 00:09:48.335605 openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      895 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-05-09 00:09:48.339605 openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      805 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/__init__.py
--rw-r--r--   0        0        0       21 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/available_indicators.py
--rw-r--r--   0        0        0    12504 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/country_profile.py
--rw-r--r--   0        0        0    20324 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/economic_indicators.py
--rw-r--r--   0        0        0       24 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/__init__.py
--rw-r--r--   0        0        0    22209 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/helpers.py
--rw-r--r--   0        0        0    24368 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/indicator_countries.json
--rw-r--r--   0        0        0     5244 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
--rw-r--r--   0        0        0     8156 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/main_indicators.py
--rw-r--r--   0        0        0    66758 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/multipliers.json
--rw-r--r--   0        0        0    87109 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/scales.json
--rw-r--r--   0        0        0    73815 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
--rw-r--r--   0        0        0    90624 2024-05-09 00:09:48.391605 openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/units.json
--rw-r--r--   0        0        0      716 2024-05-09 00:09:48.395605 openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-05-09 00:09:48.395605 openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-05-09 00:09:48.395605 openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3517 2024-05-09 00:09:48.395605 openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      538 2024-05-09 00:09:48.403605 openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-05-09 00:09:48.403605 openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-05-09 00:09:48.403605 openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-05-09 00:09:48.403605 openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-05-09 00:09:48.403605 openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0     1005 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9621 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8248 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    11033 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4379 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3878 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.459605 openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0     8255 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3068 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2955 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5909 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5904 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     2272 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6076 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     3713 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5918 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6102 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5308 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6493 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3446 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3144 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6772 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3617 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-05-09 00:09:48.463605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4286 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5050 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5826 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10613 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3521 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4220 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3270 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.467605 openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0     3126 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2980 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6344 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6720 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2720 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-05-09 00:09:48.487605 openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      988 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5138 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-05-09 00:09:48.491605 openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0     5393 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22763 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     9061 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2211 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     9171 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2376 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4974 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7327 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29027 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8337 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8417 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     9694 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5090 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3676 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12539 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3357 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6513 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     8655 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-05-09 00:09:48.495605 openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0     1840 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5105 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5157 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-05-09 00:09:48.503605 openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      981 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-05-09 00:09:48.511605 openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0     2247 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     7039 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4600 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6283 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6255 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     6204 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     9753 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_snapshots.py
--rw-r--r--   0        0        0     7150 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6142 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-05-09 00:09:48.515605 openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0     1562 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/__init__.py
--rw-r--r--   0        0        0       27 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/__init__.py
--rw-r--r--   0        0        0     1658 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/cik_map.py
--rw-r--r--   0        0        0    10150 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/company_filings.py
--rw-r--r--   0        0        0     3154 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/equity_ftd.py
--rw-r--r--   0        0        0     2681 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/equity_search.py
--rw-r--r--   0        0        0    39078 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/etf_holdings.py
--rw-r--r--   0        0        0     2820 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/form_13FHR.py
--rw-r--r--   0        0        0     2051 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/institutions_search.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/py.typed
--rw-r--r--   0        0        0     2916 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/rss_litigation.py
--rw-r--r--   0        0        0     1945 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/schema_files.py
--rw-r--r--   0        0        0     3498 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/sic_search.py
--rw-r--r--   0        0        0     1796 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/symbol_map.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/py.typed
--rw-r--r--   0        0        0       17 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/__init__.py
--rw-r--r--   0        0        0     5511 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/definitions.py
--rw-r--r--   0        0        0    12574 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/helpers.py
--rw-r--r--   0        0        0     7587 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/parse_13f.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.531605 openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/py.typed
--rw-r--r--   0        0        0      512 2024-05-09 00:09:48.619605 openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-05-09 00:09:48.619605 openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      677 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/stockgrid/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/stockgrid/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0     1120 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3651 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5295 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4662 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5323 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-05-09 00:09:48.623605 openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0     3319 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6306 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5166 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4647 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8847 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5455 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12475 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3638 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5093 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8457 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9711 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10349 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5990 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5132 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-05-09 00:09:48.635605 openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0     1241 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6582 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9222 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-05-09 00:09:48.735604 openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      440 2024-05-09 00:09:48.739604 openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     5122 2024-05-09 00:09:48.739604 openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-05-09 00:09:48.739604 openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     3719 2024-05-09 00:09:48.739604 openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0     1044 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0     4144 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2863 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3450 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3361 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6671 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5862 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3890 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10122 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4711 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4063 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10188 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4646 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4230 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6033 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-05-09 00:09:48.743605 openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0     7021 2024-05-09 00:09:59.303587 openbb_nightly-4.1.7.dev202405090009/pyproject.toml
--rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405090009/PKG-INFO
+-rw-r--r--   0        0        0     6818 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/README.md
+-rw-r--r--   0        0        0       19 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     4206 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    19033 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8326 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-05-10 00:10:03.071322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1908 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     3875 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2233 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9094 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21634 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23086 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10402 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     3064 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7595 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1948 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    66683 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     3077 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2699 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1368 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2702 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1675 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8297 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    19696 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-05-10 00:10:03.075322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0      766 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      732 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2377 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1680 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1445 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0      360 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     1027 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      902 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2321 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     2390 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-05-10 00:10:03.079322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3073 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3526 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      341 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9699 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.083322 openbb_nightly-4.1.7.dev202405100010/core/openbb_core/py.typed
+-rw-r--r--   0        0        0       34 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/commodity/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/commodity/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0       31 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/py.typed
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/__init__.py
+-rw-r--r--   0        0        0     3605 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/currency_router.py
+-rw-r--r--   0        0        0       38 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/price/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.087322 openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/py.typed
+-rw-r--r--   0        0        0       15 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1692 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0       39 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/devtools/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    12007 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.091322 openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/py.typed
+-rw-r--r--   0        0        0       19 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     2336 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     3832 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     6392 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/py.typed
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     4485 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0       23 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.095322 openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/py.typed
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/news/openbb_news/__init__.py
+-rw-r--r--   0        0        0     3213 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/news/openbb_news/news_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/news/openbb_news/py.typed
+-rw-r--r--   0        0        0       59 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0       35 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0       43 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    63911 2024-05-10 00:10:03.099322 openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0    21550 2024-05-10 00:10:03.103322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-10 00:10:03.103322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/builder.py
+-rw-r--r--   0        0        0    40926 2024-05-10 00:10:03.103322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/charting_router.py
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.103322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/__init__.py
+-rw-r--r--   0        0        0   418780 2024-05-10 00:10:03.103322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png
+-rw-r--r--   0        0        0  3585992 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js
+-rw-r--r--   0        0        0    17442 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/backend.py
+-rw-r--r--   0        0        0     7362 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/chart_style.py
+-rw-r--r--   0        0        0       42 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/config/__init__.py
+-rw-r--r--   0        0        0     8068 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py
+-rw-r--r--   0        0        0     2554 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py
+-rw-r--r--   0        0        0    58532 2024-05-10 00:10:03.119322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py
+-rw-r--r--   0        0        0  5228579 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly.html
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/__init__.py
+-rw-r--r--   0        0        0     7185 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py
+-rw-r--r--   0        0        0    12381 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py
+-rw-r--r--   0        0        0       25 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/__init__.py
+-rw-r--r--   0        0        0     8555 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py
+-rw-r--r--   0        0        0    19572 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py
+-rw-r--r--   0        0        0     3300 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py
+-rw-r--r--   0        0        0     5697 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py
+-rw-r--r--   0        0        0     6877 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py
+-rw-r--r--   0        0        0     3547 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py
+-rw-r--r--   0        0        0    25006 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py
+-rw-r--r--   0        0        0     1437 2024-05-10 00:10:03.143322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py
+-rw-r--r--   0        0        0   717892 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/table.html
+-rw-r--r--   0        0        0     2246 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/to_chart.py
+-rw-r--r--   0        0        0    26843 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/query_params.py
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/__init__.py
+-rw-r--r--   0        0        0      603 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/colors.py
+-rw-r--r--   0        0        0     3462 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json
+-rw-r--r--   0        0        0     3491 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json
+-rw-r--r--   0        0        0     2505 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/__init__.py
+-rw-r--r--   0        0        0    20295 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py
+-rw-r--r--   0        0        0     2493 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/helpers.py
+-rw-r--r--   0        0        0    16657 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py
+-rw-r--r--   0        0        0     1440 2024-05-10 00:10:03.147322 openbb_nightly-4.1.7.dev202405100010/openbb/__init__.py
+-rw-r--r--   0        0        0  1244874 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2813 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0     3299 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6510 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    12915 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/currency.py
+-rw-r--r--   0        0        0     6402 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12047 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    65943 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27681 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     2807 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    41180 2024-05-10 00:10:03.151322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   164149 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30437 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26777 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3710 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    75739 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19482 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0     7001 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11786 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/index.py
+-rw-r--r--   0        0        0    20690 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/package/regulators.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/openbb/py.typed
+-rw-r--r--   0        0        0     1106 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5294 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      877 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    18109 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6206 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0     9807 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-05-10 00:10:03.155322 openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      779 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0     1779 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8396 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9663 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8420 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4831 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     7796 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6467 2024-05-10 00:10:03.159322 openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      895 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0       24 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     4867 2024-05-10 00:10:03.167322 openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      805 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/available_indicators.py
+-rw-r--r--   0        0        0    12510 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/country_profile.py
+-rw-r--r--   0        0        0    20336 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/economic_indicators.py
+-rw-r--r--   0        0        0       24 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/__init__.py
+-rw-r--r--   0        0        0    22209 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/helpers.py
+-rw-r--r--   0        0        0    24368 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/indicator_countries.json
+-rw-r--r--   0        0        0     5244 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json
+-rw-r--r--   0        0        0     8156 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/main_indicators.py
+-rw-r--r--   0        0        0    66758 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/multipliers.json
+-rw-r--r--   0        0        0    87109 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/scales.json
+-rw-r--r--   0        0        0    73815 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json
+-rw-r--r--   0        0        0    90624 2024-05-10 00:10:03.219322 openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/units.json
+-rw-r--r--   0        0        0      716 2024-05-10 00:10:03.223322 openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-05-10 00:10:03.223322 openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-05-10 00:10:03.223322 openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3517 2024-05-10 00:10:03.223322 openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0      538 2024-05-10 00:10:03.231322 openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-05-10 00:10:03.231322 openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-05-10 00:10:03.231322 openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-05-10 00:10:03.231322 openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-05-10 00:10:03.231322 openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0     1005 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9621 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8254 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    11039 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4385 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3932 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.291322 openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0     8255 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2961 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5908 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5901 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     3208 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6082 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     3713 2024-05-10 00:10:03.295322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5924 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6114 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5314 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     6835 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6499 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3452 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3162 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6772 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     2780 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py
+-rw-r--r--   0        0        0     3623 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4304 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5056 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5832 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3291 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    10619 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3527 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4238 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3276 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2580 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.299322 openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0     3126 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     2404 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2953 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6344 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6726 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2732 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-05-10 00:10:03.319322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0     6113 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-05-10 00:10:03.323322 openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      988 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5138 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0     5393 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22763 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0     9166 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2939 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     9171 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2382 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4980 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29033 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8343 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     8423 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     9700 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5102 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-05-10 00:10:03.327322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3682 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12545 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3369 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6519 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     8655 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-05-10 00:10:03.331322 openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0     1840 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6656 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5111 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5163 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-05-10 00:10:03.339322 openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      981 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-05-10 00:10:03.343322 openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0     2247 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     7039 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4606 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6289 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6261 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     5135 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9871 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7156 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6148 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3708 2024-05-10 00:10:03.347322 openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0     1562 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/cik_map.py
+-rw-r--r--   0        0        0    10150 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/company_filings.py
+-rw-r--r--   0        0        0     3154 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/equity_ftd.py
+-rw-r--r--   0        0        0     2681 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/equity_search.py
+-rw-r--r--   0        0        0    39078 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/etf_holdings.py
+-rw-r--r--   0        0        0     2820 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/form_13FHR.py
+-rw-r--r--   0        0        0     2051 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/institutions_search.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/py.typed
+-rw-r--r--   0        0        0     2916 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/rss_litigation.py
+-rw-r--r--   0        0        0     1945 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/schema_files.py
+-rw-r--r--   0        0        0     3498 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/sic_search.py
+-rw-r--r--   0        0        0     1796 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/symbol_map.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/py.typed
+-rw-r--r--   0        0        0       17 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/__init__.py
+-rw-r--r--   0        0        0     5511 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/definitions.py
+-rw-r--r--   0        0        0    12574 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/helpers.py
+-rw-r--r--   0        0        0     7587 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/parse_13f.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.363322 openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/py.typed
+-rw-r--r--   0        0        0      512 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      677 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/stockgrid/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/stockgrid/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0     1120 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3657 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5313 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4680 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5341 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-10 00:10:03.455322 openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0     3319 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6306 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5166 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4653 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8853 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5461 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12481 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3644 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5093 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8463 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9711 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10349 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5996 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5132 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38670 2024-05-10 00:10:03.467322 openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0     1241 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6588 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9228 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-10 00:10:03.567322 openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      440 2024-05-10 00:10:03.571322 openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     5128 2024-05-10 00:10:03.571322 openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     3719 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0     1044 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0     4144 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2869 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3456 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3367 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6677 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5868 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3896 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10128 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4717 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4069 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10194 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4682 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4236 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6039 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-05-10 00:10:03.575322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-05-10 00:10:03.579322 openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0     7021 2024-05-10 00:10:15.551318 openbb_nightly-4.1.7.dev202405100010/pyproject.toml
+-rw-r--r--   0        0        0     9528 1970-01-01 00:00:00.000000 openbb_nightly-4.1.7.dev202405100010/PKG-INFO
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/README.md` & `openbb_nightly-4.1.7.dev202405100010/README.md`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/app_loader.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/app_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/auth/user.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/dependency/coverage.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/dependency/system.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/rest_api.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/commands.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/coverage.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/api/router/user.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/command_runner.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/command_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,39 +300,46 @@
     @classmethod
     def _chart(
         cls,
         obbject: OBBject,
         **kwargs,
     ) -> None:
         """Create a chart from the command output."""
-        if "charting" not in obbject.accessors:
-            raise OpenBBError(
-                "Charting is not installed. Please install `openbb-charting`."
-            )
-        chart_params = {}
-        extra_params = kwargs.get("extra_params", {})
+        try:
+            if "charting" not in obbject.accessors:
+                raise OpenBBError(
+                    "Charting is not installed. Please install `openbb-charting`."
+                )
+            chart_params = {}
+            extra_params = kwargs.get("extra_params", {})
 
-        if hasattr(extra_params, "__dict__") and hasattr(extra_params, "chart_params"):
-            chart_params = kwargs["extra_params"].__dict__.get("chart_params", {})
-        elif isinstance(extra_params, dict) and "chart_params" in extra_params:
-            chart_params = kwargs["extra_params"].get("chart_params", {})
-
-        if "chart_params" in kwargs and kwargs["chart_params"] is not None:
-            chart_params.update(kwargs.pop("chart_params", {}))
-
-        if (
-            "kwargs" in kwargs
-            and "chart_params" in kwargs["kwargs"]
-            and kwargs["kwargs"].get("chart_params") is not None
-        ):
-            chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
-
-        if chart_params:
-            kwargs.update(chart_params)
-        obbject.charting.show(render=False, **kwargs)
+            if hasattr(extra_params, "__dict__") and hasattr(
+                extra_params, "chart_params"
+            ):
+                chart_params = kwargs["extra_params"].__dict__.get("chart_params", {})
+            elif isinstance(extra_params, dict) and "chart_params" in extra_params:
+                chart_params = kwargs["extra_params"].get("chart_params", {})
+
+            if "chart_params" in kwargs and kwargs["chart_params"] is not None:
+                chart_params.update(kwargs.pop("chart_params", {}))
+
+            if (
+                "kwargs" in kwargs
+                and "chart_params" in kwargs["kwargs"]
+                and kwargs["kwargs"].get("chart_params") is not None
+            ):
+                chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
+
+            if chart_params:
+                kwargs.update(chart_params)
+            obbject.charting.show(render=False, **kwargs)
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            if Env().DEBUG_MODE:
+                raise OpenBBError(e) from e
+            warn(str(e), OpenBBWarning)
 
     # pylint: disable=R0913, R0914
     @classmethod
     async def _execute_func(
         cls,
         route: str,
         args: Tuple[Any, ...],
@@ -445,14 +452,15 @@
                     duration=duration,
                     route=route,
                     timestamp=timestamp,
                 )
             except Exception as e:
                 if Env().DEBUG_MODE:
                     raise OpenBBError(e) from e
+                warn(str(e), OpenBBWarning)
 
         return obbject
 
 
 class CommandRunner:
     """Command runner."""
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/deprecation.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/extension_loader.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/handlers_manager.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/logging_service.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/logging_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/models/logging_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/utils/expired_files.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/logs/utils/utils.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/abstract/singleton.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/api_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/api_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/charts/chart.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/charts/charting_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/credentials.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/credentials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/example.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/extension.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/field.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/field.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/hub/hub_session.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/metadata.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/obbject.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/preferences.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/profile.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/python_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/python_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/system_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/model/user_settings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/provider_interface.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/provider_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,25 +249,32 @@
         query: bool = False,
         force_optional: bool = False,
     ) -> DataclassField:
         new_name = name.replace(".", "_")
         annotation = field.annotation
 
         additional_description = ""
-        if (extra := field.json_schema_extra) and (
-            multiple := extra.get("multiple_items_allowed")  # type: ignore
-        ):
-            if provider_name:
-                additional_description += " Multiple comma separated items allowed."
-            else:
-                additional_description += (
-                    " Multiple comma separated items allowed for provider(s): "
-                    + ", ".join(multiple)  # type: ignore[arg-type]
-                    + "."
-                )
+        if extra := field.json_schema_extra:
+            providers = []
+            for p, v in extra.items():  # type: ignore[union-attr]
+                if isinstance(v, dict) and v.get("multiple_items_allowed"):
+                    providers.append(p)
+                elif isinstance(v, list) and "multiple_items_allowed" in v:
+                    # For backwards compatibility, before this was a list
+                    providers.append(p)
+
+            if providers:
+                if provider_name:
+                    additional_description += " Multiple comma separated items allowed."
+                else:
+                    additional_description += (
+                        " Multiple comma separated items allowed for provider(s): "
+                        + ", ".join(providers)  # type: ignore[arg-type]
+                        + "."
+                    )
 
         provider_field = (
             f"(provider: {provider_name})" if provider_name != "openbb" else ""
         )
         description = (
             f"{field.description}{additional_description} {provider_field}"
             if provider_name and field.description
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/query.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/router.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/auth_service.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/hub_service.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/system_service.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/service/user_service.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/service/user_service.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/account.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/account.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/app_factory.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/container.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/coverage.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/package_builder.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/package_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -860,15 +860,23 @@
     def get_expanded_type(
         cls,
         field_name: str,
         extra: Optional[dict] = None,
         original_type: Optional[type] = None,
     ) -> object:
         """Expand the original field type."""
-        if extra and "multiple_items_allowed" in extra:
+        if extra and any(
+            (
+                v.get("multiple_items_allowed")
+                if isinstance(v, dict)
+                # For backwards compatibility, before this was a list
+                else "multiple_items_allowed" in v
+            )
+            for v in extra.values()
+        ):
             if original_type is None:
                 raise ValueError(
                     "multiple_items_allowed requires the original type to be specified."
                 )
             return List[original_type]  # type: ignore
         return cls.TYPE_EXPANSION.get(field_name, ...)
 
@@ -1446,14 +1454,18 @@
             List of dictionaries containing the field name, type, description, default,
             optional flag and standard flag for each provider.
         """
         provider_field_params = []
         expanded_types = MethodDefinition.TYPE_EXPANSION
         model_map = cls.pi.map[model]
 
+        # TODO: Change this to read the package data instead of pi.map directly
+        # We change some items (types, descriptions), so the reference.json
+        # does not reflect entirely the package code.
+
         for field, field_info in model_map[provider][params_type]["fields"].items():
             # Determine the field type, expanding it if necessary and if params_type is "Parameters"
             field_type = field_info.annotation
             is_required = field_info.is_required()
             field_type = DocstringGenerator.get_field_type(
                 field_type, is_required, "website"
             )
@@ -1466,20 +1478,26 @@
 
             cleaned_description = (
                 str(field_info.description)
                 .strip().replace("\n", " ").replace("  ", " ").replace('"', "'")
             )  # fmt: skip
 
             # Add information for the providers supporting multiple symbols
-            if params_type == "QueryParams" and field_info.json_schema_extra:
-                multiple_items_list = field_info.json_schema_extra.get(
-                    "multiple_items_allowed", None
-                )
-                if multiple_items_list:
-                    multiple_items = ", ".join(multiple_items_list)
+            if params_type == "QueryParams" and (extra := field_info.json_schema_extra):
+
+                providers = []
+                for p, v in extra.items():  # type: ignore[union-attr]
+                    if isinstance(v, dict) and v.get("multiple_items_allowed"):
+                        providers.append(p)
+                    elif isinstance(v, list) and "multiple_items_allowed" in v:
+                        # For backwards compatibility, before this was a list
+                        providers.append(p)
+
+                if providers:
+                    multiple_items = ", ".join(providers)
                     cleaned_description += (
                         f" Multiple items allowed for provider(s): {multiple_items}."
                     )
                     # Manually setting to List[<field_type>] for multiple items
                     # Should be removed if TYPE_EXPANSION is updated to include this
                     field_type = f"Union[{field_type}, List[{field_type}]]"
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/reference_loader.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/decorators.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/filters.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 """OpenBB filters."""
 
-from typing import Dict, List, Optional
+from typing import Any, Dict, Optional
 
 from openbb_core.app.utils import check_single_item, convert_to_basemodel
 
 
 def filter_inputs(
     data_processing: bool = False,
-    info: Optional[Dict[str, Dict[str, List[str]]]] = None,
+    info: Optional[Dict[str, Dict[str, Any]]] = None,
     **kwargs,
 ) -> dict:
     """Filter command inputs."""
     for key, value in kwargs.items():
         if data_processing and key == "data":
             kwargs[key] = convert_to_basemodel(value)
 
     if info:
-        PROPERTY = "multiple_items_allowed"
-
         # Here we check if list items are passed and multiple items allowed for
         # the given provider/input combination. In that case we transform the list
         # into a comma-separated string
-        for field, props in info.items():
-            if PROPERTY in props and (
-                provider := kwargs.get("provider_choices", {}).get("provider")
-            ):
-                for p in ("standard_params", "extra_params"):
-                    if field in kwargs.get(p, {}):
-                        current = kwargs[p][field]
-                        new = (
-                            ",".join(map(str, current))
-                            if isinstance(current, list)
-                            else current
+        provider = kwargs.get("provider_choices", {}).get("provider")
+        for field, properties in info.items():
+
+            for p in ("standard_params", "extra_params"):
+                if field in kwargs.get(p, {}):
+                    current = kwargs[p][field]
+                    new = (
+                        ",".join(map(str, current))
+                        if isinstance(current, list)
+                        else current
+                    )
+
+                    provider_properties = properties.get(provider, {})
+                    if isinstance(provider_properties, dict):
+                        multiple_items_allowed = provider_properties.get(
+                            "multiple_items_allowed"
                         )
+                    elif isinstance(provider_properties, list):
+                        # For backwards compatibility, before this was a list
+                        multiple_items_allowed = (
+                            "multiple_items_allowed" in provider_properties
+                        )
+                    else:
+                        multiple_items_allowed = True
 
-                        if provider and provider not in props[PROPERTY]:
-                            check_single_item(
-                                new,
-                                f"{field} -> multiple items not allowed for '{provider}'",
-                            )
+                    if not multiple_items_allowed:
+                        check_single_item(
+                            new,
+                            f"{field} -> multiple items not allowed for '{provider}'",
+                        )
 
-                        kwargs[p][field] = new
-                        break
+                    kwargs[p][field] = new
+                    break
     else:
         provider = kwargs.get("provider_choices", {}).get("provider")
         for param_category in ("standard_params", "extra_params"):
             if param_category in kwargs:
                 for field, value in kwargs[param_category].items():
                     if isinstance(value, list):
                         kwargs[param_category][field] = ",".join(map(str, value))
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/static/utils/linters.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/utils.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/app/version.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/env.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/data.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/fetcher.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/provider.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/abstract/query_params.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/abstract/query_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,32 @@
     - Alias handling: Utilizes an aliasing mechanism to maintain compatibility with different naming
         conventions across various data formats. The alias is only applied when running `model_dump`.
     - Json schema extra merging:
 
         Merge different json schema extra, identified by provider.
         Example:
             FMP fetcher:
-                __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+                __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
             Intrinio fetcher
-                __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+                __json_schema_extra__ = {"symbol": {"multiple_items_allowed": False}}
 
-            Creates a new field in the `symbol` schema with:
+            Creates new fields in the `symbol` schema:
             {
-                ...,
-                "multiple_items_allowed": ["fmp", "intrinio"],
+                "type": "string",
+                "description": "Symbol to get data for.",
+                "fmp": {"multiple_items_allowed": True},
+                "intrinio": {"multiple_items_allowed": False}
                 ...,
             }
 
         Multiple fields can be tagged with the same or multiple properties.
         Example:
         __json_schema_extra__ = {
-            "<field_name_A>": ["some_prop", "another_prop"],
-            "<field_name_B>": ["yet_another_prop"]
+            "<field_name_A>": {"foo": 123, "bar": 456},
+            "<field_name_B>": {"foo": 789}
         }
 
     Attributes:
     __alias_dict__ (Dict[str, str]):
         A dictionary that maps field names to their aliases,
         facilitating the use of different naming conventions.
     __json_schema_extra__ (Dict[str, List[str]]):
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/query_executor.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/registry.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/registry.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/registry_map.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/registry_map.py`

 * *Files 15% similar despite different names*

```diff
@@ -100,46 +100,42 @@
                             "query": self._get_model(fetcher, "query_params"),
                             "data": self._get_model(fetcher, "data"),
                             "results_type": self._get_results_type(fetcher),
                         }
                     }
                 )
 
-                self._merge_json_schema_extra(p, fetcher, standard_extra[model_name])
+                self._update_json_schema_extra(p, fetcher, standard_extra[model_name])
 
         return standard_extra, original_models
 
-    def _merge_json_schema_extra(
+    def _update_json_schema_extra(
         self,
         provider: str,
         fetcher: Fetcher,
         model_map: dict,
     ):
         """Merge json schema extra for different providers."""
         model: BaseModel = RegistryMap._get_model(fetcher, "query_params")
-        std_fields = model_map["openbb"]["QueryParams"]["fields"]
+        standard_fields = model_map["openbb"]["QueryParams"]["fields"]
         extra_fields = model_map[provider]["QueryParams"]["fields"]
-        for f, props in getattr(model, "__json_schema_extra__", {}).items():
-            for p in props:
-                if f in std_fields:
-                    model_field = std_fields[f]
-                elif f in extra_fields:
-                    model_field = extra_fields[f]
+
+        for field, properties in getattr(model, "__json_schema_extra__", {}).items():
+            if properties:
+                if field in standard_fields:
+                    model_field = standard_fields[field]
+                elif field in extra_fields:
+                    model_field = extra_fields[field]
                 else:
                     continue
 
                 if model_field.json_schema_extra is None:
                     model_field.json_schema_extra = {}
 
-                if p not in model_field.json_schema_extra:
-                    model_field.json_schema_extra[p] = []
-
-                providers = model_field.json_schema_extra[p]
-                if provider not in providers:
-                    providers.append(provider)
+                model_field.json_schema_extra[provider] = properties
 
     def _get_models(self, map_: MapType) -> List[str]:
         """Get available models."""
         return list(map_.keys())
 
     @staticmethod
     def _get_results_type(fetcher: Fetcher) -> Any:
@@ -148,41 +144,46 @@
 
     @staticmethod
     def _extract_info(
         fetcher: Fetcher, type_: Literal["query_params", "data"]
     ) -> tuple:
         """Extract info (fields and docstring) from fetcher query params or data."""
         model: BaseModel = RegistryMap._get_model(fetcher, type_)
-        all_fields = {}
         standard_info: Dict[str, Any] = {"fields": {}, "docstring": None}
-        found_top_level = False
+        extra_info: Dict[str, Any] = {"fields": {}, "docstring": model.__doc__}
+        found_first_standard = False
 
-        for c in RegistryMap._class_hierarchy(model):
-            if c.__name__ in SKIP:
+        family = RegistryMap._get_class_family(model)
+        for i, child in enumerate(family):
+            if child.__name__ in SKIP:
                 continue
-            if (Path(getfile(c)).parent == STANDARD_MODELS_FOLDER) or found_top_level:
-                if not found_top_level:
-                    # We might update the standard_info more than once to account for
-                    # nested standard models, but we only want to update the docstring
-                    # once with the __doc__ of the top-level standard model.
-                    standard_info["docstring"] = c.__doc__
-                    found_top_level = True
-                standard_info["fields"].update(c.model_fields)
-            else:
-                all_fields.update(c.model_fields)
 
-        extra_info: Dict[str, Any] = {
-            "fields": {},
-            "docstring": model.__doc__,
-        }
-
-        # We ignore fields that are already in the standard model
-        for name, field in all_fields.items():
-            if name not in standard_info["fields"]:
-                extra_info["fields"][name] = field
+            parent = family[i + 1] if family[i + 1] not in SKIP else BaseModel
+
+            fields = {
+                name: field
+                for name, field in child.model_fields.items()
+                # This ensures fields inherited by c are discarded.
+                # We need to compare child and parent __annotations__
+                # because this attribute is redirected to the parent class
+                # when the child simply inherits the parent and does not
+                # define any attributes.
+                # TLDR: Only fields defined in c are included
+                if name in child.__annotations__
+                and child.__annotations__ is not parent.__annotations__
+            }
+
+            if Path(getfile(child)).parent == STANDARD_MODELS_FOLDER:
+                if not found_first_standard:
+                    # If standard uses inheritance we just use the first docstring
+                    standard_info["docstring"] = child.__doc__
+                    found_first_standard = True
+                standard_info["fields"].update(fields)
+            else:
+                extra_info["fields"].update(fields)
 
         return standard_info, extra_info
 
     @staticmethod
     def _get_model(
         fetcher: Fetcher, type_: Literal["query_params", "data"]
     ) -> BaseModel:
@@ -200,10 +201,10 @@
             raise ValueError(
                 f"'{model_str}' must be a subclass of '{parent_model.__name__}'.\n"
                 "If you are returning a nested type, try specifying"
                 f" `{type_}_type = <'your_{type_}_type'>` in the fetcher."
             )
 
     @staticmethod
-    def _class_hierarchy(class_) -> tuple:
-        """Return the class hierarchy starting with the class itself until `object`."""
+    def _get_class_family(class_) -> tuple:
+        """Return the class family starting with the class itself until `object`."""
         return getattr(class_, "__mro__", ())
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/available_indices.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_reference.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/bond_trades.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cik_map.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_filings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/company_overview.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cot.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cot_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/country_profile.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cp.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/cpi.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_info.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_performance.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_score.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/esg_sector.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_info.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_performance.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fred_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/fred_series.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/hqm.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/income_statement.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_info.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_search.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/industry_pe.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/key_executives.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_indices.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_movers.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/money_measures.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/moody.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/options_chains.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/price_target.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/recent_performance.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/search_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sector_pe.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/short_volume.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/spot.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/tbffr.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/tmc.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/top_retail.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/unemployment.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/standard_models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/client.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/descriptions.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/core/openbb_core/provider/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/core/openbb_core/provider/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/commodity/openbb_commodity/commodity_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/commodity/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/crypto_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/crypto/openbb_crypto/price/price_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/crypto/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/currency_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/currency_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,26 +17,22 @@
 router.include_router(price_router)
 
 
 # pylint: disable=unused-argument
 @router.command(
     model="CurrencyPairs",
     examples=[
-        APIEx(parameters={"provider": "intrinio"}),
+        APIEx(parameters={"provider": "fmp"}),
         APIEx(
-            description="Search for 'EURUSD' currency pair using 'intrinio' as provider.",
-            parameters={"provider": "intrinio", "symbol": "EURUSD"},
-        ),
-        APIEx(
-            description="Search for actively traded currency pairs on the queried date using 'polygon' as provider.",
-            parameters={"provider": "polygon", "date": "2024-01-02", "active": True},
+            description="Search for 'EUR' currency pair using 'intrinio' as provider.",
+            parameters={"provider": "intrinio", "query": "EUR"},
         ),
         APIEx(
             description="Search for terms  using 'polygon' as provider.",
-            parameters={"provider": "polygon", "search": "Euro zone"},
+            parameters={"provider": "polygon", "query": "Euro zone"},
         ),
     ],
 )
 async def search(
     cc: CommandContext,
     provider_choices: ProviderChoices,
     standard_params: StandardParams,
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/currency/openbb_currency/price/price_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/currency/openbb_currency/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/futures/futures_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/derivatives/openbb_derivatives/options/options_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/derivatives/openbb_derivatives/options/options_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/econometrics_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/econometrics/openbb_econometrics/utils.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/econometrics/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/economy_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/economy_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/economy/openbb_economy/gdp/gdp_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/economy/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/calendar/calendar_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/compare/compare_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/compare/compare_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/darkpool/darkpool_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/equity_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/estimates/estimates_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/estimates/estimates_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/fundamental/fundamental_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/ownership/ownership_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/price/price_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/equity/openbb_equity/shorts/shorts_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/equity/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/discovery/discovery_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/etf/openbb_etf/etf_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/etf/openbb_etf/etf_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/government/government_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/government/government_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/fixedincome/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/index_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/index/openbb_index/price/price_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/index/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/news/openbb_news/news_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/news/openbb_news/news_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/models.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/performance/performance_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/quantitative_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/statistics.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/quantitative/openbb_quantitative/stats/stats_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/quantitative/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/cftc/cftc_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/regulators/openbb_regulators/sec/sec_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/regulators/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/extensions/technical/openbb_technical/technical_router.py` & `openbb_nightly-4.1.7.dev202405100010/extensions/technical/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/builder.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/builder.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/charting_router.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/charting_router.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/assets/Terminal_icon.png`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/assets/plotly-2.24.2.min.js`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/backend.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/chart_style.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/chart_style.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/config/openbb_styles.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/dummy_backend.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/dummy_backend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/openbb_figure.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/openbb_figure.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly.html` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/data_classes.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/custom_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/momentum_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/trend_indicators_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volatility_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/plugins/volume_plugin.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_class.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/plotly_ta/ta_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/table.html` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/table.html`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/core/to_chart.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/core/to_chart.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/query_params.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/colors.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/colors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/dark.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/light.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/styles/default/tables.pltstyle.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/generic_charts.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/generic_charts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py` & `openbb_nightly-4.1.7.dev202405100010/obbject_extensions/charting/openbb_charting/utils/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/assets/reference.json` & `openbb_nightly-4.1.7.dev202405100010/openbb/assets/reference.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998348243811414%*

 * *Differences: {"'paths'": '{\'/currency/search\': {\'examples\': "\\nExamples\\n--------\\n\\n```python\\nfrom '*

 * *            "openbb import obb\\nobb.currency.search(provider='fmp')\\n# Search for 'EUR' currency "*

 * *            "pair using 'intrinio' as provider.\\nobb.currency.search(provider='intrinio', "*

 * *            "query='EUR')\\n# Search for terms  using 'polygon' as "*

 * *            "provider.\\nobb.currency.search(provider='polygon', query='Euro "*

 * *            'zone\')\\n```\\n\\n", \'parameters\': {\'standard\': {inse […]*

```diff
@@ -601,21 +601,14 @@
                         "optional": true,
                         "type": "str"
                     }
                 ],
                 "intrinio": [
                     {
                         "default": "",
-                        "description": "Code of the currency pair.",
-                        "name": "code",
-                        "optional": false,
-                        "type": "str"
-                    },
-                    {
-                        "default": "",
                         "description": "ISO 4217 currency code of the base currency.",
                         "name": "base_currency",
                         "optional": false,
                         "type": "str"
                     },
                     {
                         "default": "",
@@ -623,143 +616,100 @@
                         "name": "quote_currency",
                         "optional": false,
                         "type": "str"
                     }
                 ],
                 "polygon": [
                     {
-                        "default": "",
-                        "description": "Name of the trading market. Always 'fx'.",
-                        "name": "market",
-                        "optional": false,
-                        "type": "str"
-                    },
-                    {
-                        "default": "",
-                        "description": "Locale of the currency pair.",
-                        "name": "locale",
-                        "optional": false,
-                        "type": "str"
-                    },
-                    {
                         "default": null,
                         "description": "The symbol of the quote currency.",
                         "name": "currency_symbol",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
-                        "description": "Name of the quote currency.",
-                        "name": "currency_name",
-                        "optional": true,
-                        "type": "str"
-                    },
-                    {
-                        "default": null,
                         "description": "The symbol of the base currency.",
                         "name": "base_currency_symbol",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
                         "description": "Name of the base currency.",
                         "name": "base_currency_name",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": "",
-                        "description": "The last updated timestamp in UTC.",
-                        "name": "last_updated_utc",
+                        "description": "Name of the trading market. Always 'fx'.",
+                        "name": "market",
                         "optional": false,
-                        "type": "datetime"
+                        "type": "str"
+                    },
+                    {
+                        "default": "",
+                        "description": "Locale of the currency pair.",
+                        "name": "locale",
+                        "optional": false,
+                        "type": "str"
                     },
                     {
                         "default": null,
-                        "description": "The delisted timestamp in UTC.",
-                        "name": "delisted_utc",
+                        "description": "The date the reference data was last updated.",
+                        "name": "last_updated",
                         "optional": true,
-                        "type": "datetime"
+                        "type": "date"
+                    },
+                    {
+                        "default": null,
+                        "description": "The date the item was delisted.",
+                        "name": "delisted",
+                        "optional": true,
+                        "type": "date"
                     }
                 ],
                 "standard": [
                     {
                         "default": "",
+                        "description": "Symbol representing the entity requested in the data.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
                         "description": "Name of the currency pair.",
                         "name": "name",
-                        "optional": false,
+                        "optional": true,
                         "type": "str"
                     }
                 ]
             },
             "deprecated": {
                 "flag": null,
                 "message": null
             },
             "description": "Currency Search.\n\nSearch available currency pairs.\nCurrency pairs are the national currencies from two countries coupled for trading on\nthe foreign exchange (FX) marketplace.\nBoth currencies will have exchange rates on which the trade will have its position basis.\nAll trading within the forex market, whether selling, buying, or trading, will take place through currency pairs.\n(ref: Investopedia)\nMajor currency pairs include pairs such as EUR/USD, USD/JPY, GBP/USD, etc.",
-            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.currency.search(provider='intrinio')\n# Search for 'EURUSD' currency pair using 'intrinio' as provider.\nobb.currency.search(provider='intrinio', symbol=EURUSD)\n# Search for actively traded currency pairs on the queried date using 'polygon' as provider.\nobb.currency.search(provider='polygon', date=2024-01-02, active=True)\n# Search for terms  using 'polygon' as provider.\nobb.currency.search(provider='polygon', search=Euro zone)\n```\n\n",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.currency.search(provider='fmp')\n# Search for 'EUR' currency pair using 'intrinio' as provider.\nobb.currency.search(provider='intrinio', query='EUR')\n# Search for terms  using 'polygon' as provider.\nobb.currency.search(provider='polygon', query='Euro zone')\n```\n\n",
             "model": "CurrencyPairs",
             "parameters": {
                 "fmp": [],
                 "intrinio": [],
-                "polygon": [
-                    {
-                        "default": null,
-                        "description": "Symbol of the pair to search.",
-                        "name": "symbol",
-                        "optional": true,
-                        "type": "str"
-                    },
+                "polygon": [],
+                "standard": [
                     {
                         "default": null,
-                        "description": "A specific date to get data for.",
-                        "name": "date",
-                        "optional": true,
-                        "type": "Union[date, str]"
-                    },
-                    {
-                        "default": "",
-                        "description": "Search for terms within the ticker and/or company name.",
-                        "name": "search",
+                        "description": "Query to search for currency pairs.",
+                        "name": "query",
                         "optional": true,
                         "type": "str"
                     },
                     {
-                        "default": true,
-                        "description": "Specify if the tickers returned should be actively traded on the queried date.",
-                        "name": "active",
-                        "optional": true,
-                        "type": "bool"
-                    },
-                    {
-                        "default": "asc",
-                        "description": "Order data by ascending or descending.",
-                        "name": "order",
-                        "optional": true,
-                        "type": "Literal['asc', 'desc']"
-                    },
-                    {
-                        "default": null,
-                        "description": "Sort field used for ordering.",
-                        "name": "sort",
-                        "optional": true,
-                        "type": "Literal['ticker', 'name', 'market', 'locale', 'currency_symbol', 'currency_name', 'base_currency_symbol', 'base_currency_name', 'last_updated_utc', 'delisted_utc']"
-                    },
-                    {
-                        "default": 1000,
-                        "description": "The number of data entries to return.",
-                        "name": "limit",
-                        "optional": true,
-                        "type": "Annotated[int, Gt(gt=0)]"
-                    }
-                ],
-                "standard": [
-                    {
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon']"
                     }
                 ]
@@ -2725,14 +2675,21 @@
             },
             "description": "Query the Geo Fred API for regional economic data by series group.\n\nThe series group ID is found by using `fred_search` and the `series_id` parameter.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.economy.fred_regional(symbol='NYICLAIMS', provider='fred')\n# With a date, time series data is returned.\nobb.economy.fred_regional(symbol='NYICLAIMS', start_date='2021-01-01', end_date='2021-12-31', limit=10, provider='fred')\n```\n\n",
             "model": "FredRegional",
             "parameters": {
                 "fred": [
                     {
+                        "default": "",
+                        "description": "For this function, it is the series_group ID or series ID. If the symbol provided is for a series_group, set the `is_series_group` parameter to True. Not all series that are in FRED have geographical data.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
                         "default": false,
                         "description": "When True, the symbol provided is for a series_group, else it is for a series ID.",
                         "name": "is_series_group",
                         "optional": true,
                         "type": "bool"
                     },
                     {
@@ -3141,14 +3098,21 @@
             },
             "description": "Get data by series ID from FRED.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.economy.fred_series(symbol='NFCI', provider='fred')\n# Multiple series can be passed in as a list.\nobb.economy.fred_series(symbol='NFCI,STLFSI4', provider='fred')\n# Use the `transform` parameter to transform the data as change, log, or percent change.\nobb.economy.fred_series(symbol='CBBTCUSD', transform=pc1, provider='fred')\n```\n\n",
             "model": "FredSeries",
             "parameters": {
                 "fred": [
                     {
+                        "default": 100000,
+                        "description": "The number of data entries to return.",
+                        "name": "limit",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
                         "default": null,
                         "description": "Frequency aggregation to convert high frequency data to lower frequency.       None = No change       a = Annual       q = Quarterly       m = Monthly       w = Weekly       d = Daily       wef = Weekly, Ending Friday       weth = Weekly, Ending Thursday       wew = Weekly, Ending Wednesday       wetu = Weekly, Ending Tuesday       wem = Weekly, Ending Monday       wesu = Weekly, Ending Sunday       wesa = Weekly, Ending Saturday       bwew = Biweekly, Ending Wednesday       bwem = Biweekly, Ending Monday",
                         "name": "frequency",
                         "optional": true,
                         "type": "Literal['a', 'q', 'm', 'w', 'd', 'wef', 'weth', 'wew', 'wetu', 'wem', 'wesu', 'wesa', 'bwew', 'bwem']"
                     },
                     {
@@ -7383,14 +7347,21 @@
             }
         },
         "/equity/estimates/price_target": {
             "data": {
                 "benzinga": [
                     {
                         "default": null,
+                        "description": "Description of the change in rating from firm's last rating.Note that all of these terms are precisely defined.",
+                        "name": "action",
+                        "optional": true,
+                        "type": "Literal['Downgrades', 'Maintains', 'Reinstates', 'Reiterates', 'Upgrades', 'Assumes', 'Initiates Coverage On', 'Terminates Coverage On', 'Removes', 'Suspends', 'Firm Dissolved']"
+                    },
+                    {
+                        "default": null,
                         "description": "Description of the change in price target from firm's last price target.",
                         "name": "action_change",
                         "optional": true,
                         "type": "Literal['Announces', 'Maintains', 'Lowers', 'Raises', 'Removes', 'Adjusts']"
                     },
                     {
                         "default": null,
@@ -8950,26 +8921,48 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get the balance sheet for a given company.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.fundamental.balance(symbol='AAPL', provider='fmp')\nobb.equity.fundamental.balance(symbol='AAPL', period='annual', limit=5, provider='intrinio')\n```\n\n",
             "model": "BalanceSheet",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    },
+                    {
                         "default": null,
                         "description": "The specific fiscal year. Reports do not go beyond 2008.",
                         "name": "fiscal_year",
                         "optional": true,
                         "type": "int"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm']"
+                    },
+                    {
                         "default": null,
                         "description": "Filing date of the financial statement.",
                         "name": "filing_date",
                         "optional": true,
                         "type": "date"
                     },
                     {
@@ -9083,15 +9076,23 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'yfinance']"
                     }
                 ],
-                "yfinance": []
+                "yfinance": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[BalanceSheet]"
@@ -9483,14 +9484,21 @@
             }
         },
         "/equity/fundamental/cash": {
             "data": {
                 "fmp": [
                     {
                         "default": null,
+                        "description": "The fiscal year of the fiscal period.",
+                        "name": "fiscal_year",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "default": null,
                         "description": "The date of the filing.",
                         "name": "filing_date",
                         "optional": true,
                         "type": "date"
                     },
                     {
                         "default": null,
@@ -10170,26 +10178,48 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get the cash flow statement for a given company.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.fundamental.cash(symbol='AAPL', provider='fmp')\nobb.equity.fundamental.cash(symbol='AAPL', period='annual', limit=5, provider='intrinio')\n```\n\n",
             "model": "CashFlowStatement",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm', 'ytd']"
+                    },
+                    {
                         "default": null,
                         "description": "The specific fiscal year. Reports do not go beyond 2008.",
                         "name": "fiscal_year",
                         "optional": true,
                         "type": "int"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    },
+                    {
                         "default": null,
                         "description": "Filing date of the financial statement.",
                         "name": "filing_date",
                         "optional": true,
                         "type": "date"
                     },
                     {
@@ -10303,15 +10333,23 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'yfinance']"
                     }
                 ],
-                "yfinance": []
+                "yfinance": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[CashFlowStatement]"
@@ -11147,14 +11185,28 @@
                         "optional": true,
                         "type": "bool"
                     }
                 ],
                 "sec": [
                     {
                         "default": null,
+                        "description": "Symbol to get data for.",
+                        "name": "symbol",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
+                        "description": "Type of the SEC filing form.",
+                        "name": "form_type",
+                        "optional": true,
+                        "type": "Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']"
+                    },
+                    {
+                        "default": null,
                         "description": "Lookup filings by Central Index Key (CIK) instead of by symbol.",
                         "name": "cik",
                         "optional": true,
                         "type": "Union[int, str]"
                     },
                     {
                         "default": true,
@@ -12717,26 +12769,48 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get the income statement for a given company.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.fundamental.income(symbol='AAPL', provider='fmp')\nobb.equity.fundamental.income(symbol='AAPL', period='annual', limit=5, provider='intrinio')\n```\n\n",
             "model": "IncomeStatement",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm', 'ytd']"
+                    },
+                    {
                         "default": null,
                         "description": "The specific fiscal year. Reports do not go beyond 2008.",
                         "name": "fiscal_year",
                         "optional": true,
                         "type": "int"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm']"
+                    },
+                    {
                         "default": null,
                         "description": "Filing date of the financial statement.",
                         "name": "filing_date",
                         "optional": true,
                         "type": "date"
                     },
                     {
@@ -12850,15 +12924,23 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'yfinance']"
                     }
                 ],
-                "yfinance": []
+                "yfinance": [
+                    {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    }
+                ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[IncomeStatement]"
@@ -15802,17 +15884,32 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get an extensive set of financial and accounting ratios for a given company over time.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.fundamental.ratios(symbol='AAPL', provider='fmp')\nobb.equity.fundamental.ratios(symbol='AAPL', period='annual', limit=12, provider='intrinio')\n```\n\n",
             "model": "FinancialRatios",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "annual",
+                        "description": "Time period of the data to return.",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "annual",
+                        "description": "Time period of the data to return.",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter', 'ttm', 'ytd']"
+                    },
+                    {
                         "default": null,
                         "description": "The specific fiscal year. Reports do not go beyond 2008.",
                         "name": "fiscal_year",
                         "optional": true,
                         "type": "int"
                     }
                 ],
@@ -15910,14 +16007,28 @@
             },
             "description": "Get financial statements as reported by the company.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.fundamental.reported_financials(symbol='AAPL', provider='intrinio')\n# Get AAPL balance sheet with a limit of 10 items.\nobb.equity.fundamental.reported_financials(symbol='AAPL', period='annual', statement_type='balance', limit=10, provider='intrinio')\n# Get reported income statement\nobb.equity.fundamental.reported_financials(symbol='AAPL', statement_type='income', provider='intrinio')\n# Get reported cash flow statement\nobb.equity.fundamental.reported_financials(symbol='AAPL', statement_type='cash', provider='intrinio')\n```\n\n",
             "model": "ReportedFinancials",
             "parameters": {
                 "intrinio": [
                     {
+                        "default": "annual",
+                        "description": "None",
+                        "name": "period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    },
+                    {
+                        "default": "income",
+                        "description": "Cash flow statements are reported as YTD, Q4 is the same as FY.",
+                        "name": "statement_type",
+                        "optional": true,
+                        "type": "Literal['balance', 'income', 'cash']"
+                    },
+                    {
                         "default": null,
                         "description": "The specific fiscal year. Reports do not go beyond 2008.",
                         "name": "fiscal_year",
                         "optional": true,
                         "type": "int"
                     }
                 ],
@@ -17142,14 +17253,21 @@
                         "name": "form_type",
                         "optional": false,
                         "type": "str"
                     }
                 ],
                 "intrinio": [
                     {
+                        "default": null,
+                        "description": "URL of the filing.",
+                        "name": "filing_url",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "",
                         "description": "Name of the company.",
                         "name": "company_name",
                         "optional": false,
                         "type": "str"
                     },
                     {
@@ -18597,17 +18715,39 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get historical price data for a given stock. This includes open, high, low, close, and volume.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.price.historical(symbol='AAPL', provider='fmp')\nobb.equity.price.historical(symbol='AAPL', interval='1d', provider='intrinio')\n```\n\n",
             "model": "EquityHistorical",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '15m', '30m', '1h', '4h', '1d']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "",
+                        "description": "A Security identifier (Ticker, FIGI, ISIN, CUSIP, Intrinio ID).",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '10m', '15m', '30m', '60m', '1h', '1d', '1W', '1M', '1Q', '1Y']"
+                    },
+                    {
                         "default": null,
                         "description": "Return intervals starting at the specified time on the `start_date` formatted as 'HH:MM:SS'.",
                         "name": "start_time",
                         "optional": true,
                         "type": "datetime.time"
                     },
                     {
@@ -18630,14 +18770,21 @@
                         "name": "source",
                         "optional": true,
                         "type": "Literal['realtime', 'delayed', 'nasdaq_basic']"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return. The numeric portion of the interval can be any positive integer. The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "splits_only",
                         "description": "The adjustment factor to apply. Default is splits only.",
                         "name": "adjustment",
                         "optional": true,
                         "type": "Literal['splits_only', 'unadjusted']"
                     },
                     {
@@ -18695,17 +18842,32 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'tiingo', 'yfinance']"
                     }
                 ],
-                "tiingo": [],
+                "tiingo": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1d', '1W', '1M', '1Y']"
+                    }
+                ],
                 "yfinance": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '2m', '5m', '15m', '30m', '60m', '90m', '1h', '1d', '5d', '1W', '1M', '1Q']"
+                    },
+                    {
                         "default": false,
                         "description": "Include Pre and Post market data.",
                         "name": "extended_hours",
                         "optional": true,
                         "type": "bool"
                     },
                     {
@@ -18963,15 +19125,23 @@
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
         "/equity/price/performance": {
             "data": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "",
+                        "description": "The ticker symbol.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    }
+                ],
                 "standard": [
                     {
                         "default": null,
                         "description": "Symbol representing the entity requested in the data.",
                         "name": "symbol",
                         "optional": true,
                         "type": "str"
@@ -19514,14 +19684,21 @@
             "description": "Get the latest quote for a given stock. Quote includes price, volume, and other data.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.price.quote(symbol='AAPL', provider='fmp')\n```\n\n",
             "model": "EquityQuote",
             "parameters": {
                 "fmp": [],
                 "intrinio": [
                     {
+                        "default": "",
+                        "description": "A Security identifier (Ticker, FIGI, ISIN, CUSIP, Intrinio ID).",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
                         "default": "iex",
                         "description": "Source of the data.",
                         "name": "source",
                         "optional": true,
                         "type": "Literal['iex', 'bats', 'bats_delayed', 'utp_delayed', 'cta_a_delayed', 'cta_b_delayed', 'intrinio_mx', 'intrinio_mx_plus', 'delayed_sip']"
                     }
                 ],
@@ -21072,17 +21249,39 @@
                 "flag": null,
                 "message": null
             },
             "description": "ETF Historical Market Price.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.etf.historical(symbol='SPY', provider='fmp')\nobb.etf.historical(symbol='SPY', provider='yfinance')\n# This function accepts multiple tickers.\nobb.etf.historical(symbol='SPY,IWM,QQQ,DJIA', provider='yfinance')\n```\n\n",
             "model": "EtfHistorical",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '15m', '30m', '1h', '4h', '1d']"
+                    }
+                ],
                 "intrinio": [
                     {
+                        "default": "",
+                        "description": "A Security identifier (Ticker, FIGI, ISIN, CUSIP, Intrinio ID).",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '10m', '15m', '30m', '60m', '1h', '1d', '1W', '1M', '1Q', '1Y']"
+                    },
+                    {
                         "default": null,
                         "description": "Return intervals starting at the specified time on the `start_date` formatted as 'HH:MM:SS'.",
                         "name": "start_time",
                         "optional": true,
                         "type": "datetime.time"
                     },
                     {
@@ -21105,14 +21304,21 @@
                         "name": "source",
                         "optional": true,
                         "type": "Literal['realtime', 'delayed', 'nasdaq_basic']"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return. The numeric portion of the interval can be any positive integer. The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "splits_only",
                         "description": "The adjustment factor to apply. Default is splits only.",
                         "name": "adjustment",
                         "optional": true,
                         "type": "Literal['splits_only', 'unadjusted']"
                     },
                     {
@@ -21170,17 +21376,32 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'tiingo', 'yfinance']"
                     }
                 ],
-                "tiingo": [],
+                "tiingo": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1d', '1W', '1M', '1Y']"
+                    }
+                ],
                 "yfinance": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '2m', '5m', '15m', '30m', '60m', '90m', '1h', '1d', '5d', '1W', '1M', '1Q']"
+                    },
+                    {
                         "default": false,
                         "description": "Include Pre and Post market data.",
                         "name": "extended_hours",
                         "optional": true,
                         "type": "bool"
                     },
                     {
@@ -21393,14 +21614,21 @@
                         "optional": true,
                         "type": "Union[date, datetime]"
                     }
                 ],
                 "intrinio": [
                     {
                         "default": null,
+                        "description": "The common name for the holding.",
+                        "name": "name",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": null,
                         "description": "The type of instrument for this holding. Examples(Bond='BOND', Equity='EQUI')",
                         "name": "security_type",
                         "optional": true,
                         "type": "str"
                     },
                     {
                         "default": null,
@@ -22216,15 +22444,23 @@
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
         "/etf/holdings_performance": {
             "data": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "",
+                        "description": "The ticker symbol.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    }
+                ],
                 "standard": [
                     {
                         "default": null,
                         "description": "Symbol representing the entity requested in the data.",
                         "name": "symbol",
                         "optional": true,
                         "type": "str"
@@ -23593,15 +23829,23 @@
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
         "/etf/price_performance": {
             "data": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "",
+                        "description": "The ticker symbol.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    }
+                ],
                 "intrinio": [
                     {
                         "default": null,
                         "description": "Annualized rate of return from inception.",
                         "name": "max_annualized",
                         "optional": true,
                         "type": "float"
@@ -26250,15 +26494,23 @@
                 "flag": null,
                 "message": null
             },
             "description": "Get Index Constituents.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.index.constituents(symbol='dowjones', provider='fmp')\n```\n\n",
             "model": "IndexConstituents",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "dowjones",
+                        "description": "None",
+                        "name": "symbol",
+                        "optional": true,
+                        "type": "Literal['dowjones', 'sp500', 'nasdaq']"
+                    }
+                ],
                 "standard": [
                     {
                         "default": "",
                         "description": "Symbol to get data for.",
                         "name": "symbol",
                         "optional": false,
                         "type": "str"
@@ -26387,26 +26639,41 @@
                 "flag": true,
                 "message": "This endpoint is deprecated; use `/index/price/historical` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.3."
             },
             "description": "Get Historical Market Indices.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.index.market(symbol='^IBEX', provider='fmp')\n```\n\n",
             "model": "MarketIndices",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '15m', '30m', '1h', '4h', '1d']"
+                    }
+                ],
                 "intrinio": [
                     {
                         "default": 10000,
                         "description": "The number of data entries to return.",
                         "name": "limit",
                         "optional": true,
                         "type": "int"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return. The numeric portion of the interval can be any positive integer. The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "asc",
                         "description": "Sort order of the data. This impacts the results in combination with the 'limit' parameter. The results are always returned in ascending order by date.",
                         "name": "sort",
                         "optional": true,
                         "type": "Literal['asc', 'desc']"
                     },
                     {
@@ -26450,15 +26717,23 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'yfinance']"
                     }
                 ],
-                "yfinance": []
+                "yfinance": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '2m', '5m', '15m', '30m', '60m', '90m', '1h', '1d', '5d', '1W', '1M', '1Q']"
+                    }
+                ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[MarketIndices]"
@@ -26571,26 +26846,41 @@
                 "flag": null,
                 "message": null
             },
             "description": "Historical Index Levels.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.index.price.historical(symbol='^GSPC', provider='fmp')\n# Not all providers have the same symbols.\nobb.index.price.historical(symbol='SPX', provider='intrinio')\n```\n\n",
             "model": "IndexHistorical",
             "parameters": {
-                "fmp": [],
+                "fmp": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '5m', '15m', '30m', '1h', '4h', '1d']"
+                    }
+                ],
                 "intrinio": [
                     {
                         "default": 10000,
                         "description": "The number of data entries to return.",
                         "name": "limit",
                         "optional": true,
                         "type": "int"
                     }
                 ],
                 "polygon": [
                     {
+                        "default": "1d",
+                        "description": "Time interval of the data to return. The numeric portion of the interval can be any positive integer. The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
                         "default": "asc",
                         "description": "Sort order of the data. This impacts the results in combination with the 'limit' parameter. The results are always returned in ascending order by date.",
                         "name": "sort",
                         "optional": true,
                         "type": "Literal['asc', 'desc']"
                     },
                     {
@@ -26634,15 +26924,23 @@
                         "default": "fmp",
                         "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
                         "name": "provider",
                         "optional": true,
                         "type": "Literal['fmp', 'intrinio', 'polygon', 'yfinance']"
                     }
                 ],
-                "yfinance": []
+                "yfinance": [
+                    {
+                        "default": "1d",
+                        "description": "Time interval of the data to return.",
+                        "name": "interval",
+                        "optional": true,
+                        "type": "Literal['1m', '2m', '5m', '15m', '30m', '60m', '90m', '1h', '1d', '5d', '1W', '1M', '1Q']"
+                    }
+                ]
             },
             "returns": {
                 "OBBject": [
                     {
                         "description": "Serializable results.",
                         "name": "results",
                         "type": "List[IndexHistorical]"
@@ -26670,14 +26968,21 @@
                 ]
             }
         },
         "/news/company": {
             "data": {
                 "benzinga": [
                     {
+                        "default": null,
+                        "description": "URL to the images of the news.",
+                        "name": "images",
+                        "optional": true,
+                        "type": "List[Dict[str, str]]"
+                    },
+                    {
                         "default": "",
                         "description": "Article ID.",
                         "name": "id",
                         "optional": false,
                         "type": "str"
                     },
                     {
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/__extensions__.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/crypto.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/crypto.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/crypto_price.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/crypto_price.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,17 +133,15 @@
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "fmp",
-                            "polygon",
-                            "tiingo",
-                            "yfinance",
-                        ]
+                        "fmp": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "tiingo": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/currency.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/currency.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,18 @@
 
         return currency_price.ROUTER_currency_price(command_runner=self._command_runner)
 
     @exception_handler
     @validate
     def search(
         self,
+        query: Annotated[
+            Optional[str],
+            OpenBBField(description="Query to search for currency pairs."),
+        ] = None,
         provider: Annotated[
             Optional[Literal["fmp", "intrinio", "polygon"]],
             OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
@@ -48,32 +52,20 @@
         All trading within the forex market, whether selling, buying, or trading, will take place through currency pairs.
         (ref: Investopedia)
         Major currency pairs include pairs such as EUR/USD, USD/JPY, GBP/USD, etc.
 
 
         Parameters
         ----------
+        query : Optional[str]
+            Query to search for currency pairs.
         provider : Optional[Literal['fmp', 'intrinio', 'polygon']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
-        symbol : Optional[str]
-            Symbol of the pair to search. (provider: polygon)
-        date : Optional[datetime.date]
-            A specific date to get data for. (provider: polygon)
-        search : Optional[str]
-            Search for terms within the ticker and/or company name. (provider: polygon)
-        active : Optional[bool]
-            Specify if the tickers returned should be actively traded on the queried date. (provider: polygon)
-        order : Optional[Literal['asc', 'desc']]
-            Order data by ascending or descending. (provider: polygon)
-        sort : Optional[Literal['ticker', 'name', 'market', 'locale', 'currency_symbol', 'currency_name', 'base_currency_symbol', 'base_currency_name', 'last_updated_utc', 'delisted_utc']]
-            Sort field used for ordering. (provider: polygon)
-        limit : Optional[Annotated[int, Gt(gt=0)]]
-            The number of data entries to return. (provider: polygon)
 
         Returns
         -------
         OBBject
             results : List[CurrencyPairs]
                 Serializable results.
             provider : Optional[Literal['fmp', 'intrinio', 'polygon']]
@@ -83,70 +75,66 @@
             chart : Optional[Chart]
                 Chart object.
             extra : Dict[str, Any]
                 Extra info.
 
         CurrencyPairs
         -------------
-        name : str
+        symbol : str
+            Symbol representing the entity requested in the data.
+        name : Optional[str]
             Name of the currency pair.
-        symbol : Optional[str]
-            Symbol of the currency pair. (provider: fmp)
         currency : Optional[str]
             Base currency of the currency pair. (provider: fmp)
         stock_exchange : Optional[str]
             Stock exchange of the currency pair. (provider: fmp)
         exchange_short_name : Optional[str]
             Short name of the stock exchange of the currency pair. (provider: fmp)
-        code : Optional[str]
-            Code of the currency pair. (provider: intrinio)
         base_currency : Optional[str]
             ISO 4217 currency code of the base currency. (provider: intrinio)
         quote_currency : Optional[str]
             ISO 4217 currency code of the quote currency. (provider: intrinio)
-        market : Optional[str]
-            Name of the trading market. Always 'fx'. (provider: polygon)
-        locale : Optional[str]
-            Locale of the currency pair. (provider: polygon)
         currency_symbol : Optional[str]
             The symbol of the quote currency. (provider: polygon)
-        currency_name : Optional[str]
-            Name of the quote currency. (provider: polygon)
         base_currency_symbol : Optional[str]
             The symbol of the base currency. (provider: polygon)
         base_currency_name : Optional[str]
             Name of the base currency. (provider: polygon)
-        last_updated_utc : Optional[datetime]
-            The last updated timestamp in UTC. (provider: polygon)
-        delisted_utc : Optional[datetime]
-            The delisted timestamp in UTC. (provider: polygon)
+        market : Optional[str]
+            Name of the trading market. Always 'fx'. (provider: polygon)
+        locale : Optional[str]
+            Locale of the currency pair. (provider: polygon)
+        last_updated : Optional[date]
+            The date the reference data was last updated. (provider: polygon)
+        delisted : Optional[date]
+            The date the item was delisted. (provider: polygon)
 
         Examples
         --------
         >>> from openbb import obb
-        >>> obb.currency.search(provider='intrinio')
-        >>> # Search for 'EURUSD' currency pair using 'intrinio' as provider.
-        >>> obb.currency.search(provider='intrinio', symbol='EURUSD')
-        >>> # Search for actively traded currency pairs on the queried date using 'polygon' as provider.
-        >>> obb.currency.search(provider='polygon', date='2024-01-02', active=True)
+        >>> obb.currency.search(provider='fmp')
+        >>> # Search for 'EUR' currency pair using 'intrinio' as provider.
+        >>> obb.currency.search(provider='intrinio', query='EUR')
         >>> # Search for terms  using 'polygon' as provider.
-        >>> obb.currency.search(provider='polygon', search='Euro zone')
+        >>> obb.currency.search(provider='polygon', query='Euro zone')
         """  # noqa: E501
 
         return self._run(
             "/currency/search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/currency/search",
                         ("fmp", "intrinio", "polygon"),
                     )
                 },
-                standard_params={},
+                standard_params={
+                    "query": query,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def snapshots(
@@ -298,10 +286,15 @@
                 },
                 standard_params={
                     "base": base,
                     "quote_type": quote_type,
                     "counter_currencies": counter_currencies,
                 },
                 extra_params=kwargs,
-                info={"base": {"multiple_items_allowed": ["fmp", "polygon"]}},
+                info={
+                    "base": {
+                        "fmp": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                    }
+                },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/currency_price.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/currency_price.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,17 +136,15 @@
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "fmp",
-                            "polygon",
-                            "tiingo",
-                            "yfinance",
-                        ]
+                        "fmp": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "tiingo": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/derivatives.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/derivatives_options.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/derivatives_options.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/economy.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/economy.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,17 @@
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                info={"country": {"multiple_items_allowed": ["tradingeconomics"]}},
+                info={
+                    "country": {"tradingeconomics": {"multiple_items_allowed": True}}
+                },
             )
         )
 
     @exception_handler
     @validate
     def composite_leading_indicator(
         self,
@@ -426,15 +428,15 @@
                         ("econdb",),
                     )
                 },
                 standard_params={
                     "country": country,
                 },
                 extra_params=kwargs,
-                info={"country": {"multiple_items_allowed": ["econdb"]}},
+                info={"country": {"econdb": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def cpi(
         self,
@@ -599,15 +601,15 @@
                     "units": units,
                     "frequency": frequency,
                     "harmonized": harmonized,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
-                info={"country": {"multiple_items_allowed": ["fred"]}},
+                info={"country": {"fred": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def fred_regional(
         self,
@@ -1020,15 +1022,15 @@
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fred"]}},
+                info={"symbol": {"fred": {"multiple_items_allowed": True}}},
             )
         )
 
     @property
     def gdp(self):
         # pylint: disable=import-outside-toplevel
         from . import economy_gdp
@@ -1150,16 +1152,16 @@
                     "symbol": symbol,
                     "country": country,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
                 info={
-                    "symbol": {"multiple_items_allowed": ["econdb"]},
-                    "country": {"multiple_items_allowed": ["econdb"]},
+                    "symbol": {"econdb": {"multiple_items_allowed": True}},
+                    "country": {"econdb": {"multiple_items_allowed": True}},
                 },
             )
         )
 
     @exception_handler
     @validate
     def long_term_interest_rate(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/economy_gdp.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/economy_gdp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,15 +432,17 @@
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_calendar.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_compare.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_compare.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_discovery.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_discovery.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_estimates.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,19 +218,19 @@
                 },
                 standard_params={
                     "analyst_name": analyst_name,
                     "firm_name": firm_name,
                 },
                 extra_params=kwargs,
                 info={
-                    "analyst_name": {"multiple_items_allowed": ["benzinga"]},
-                    "firm_name": {"multiple_items_allowed": ["benzinga"]},
-                    "analyst_ids": {"multiple_items_allowed": ["benzinga"]},
-                    "firm_ids": {"multiple_items_allowed": ["benzinga"]},
-                    "fields": {"multiple_items_allowed": ["benzinga"]},
+                    "analyst_name": {"benzinga": {"multiple_items_allowed": True}},
+                    "firm_name": {"benzinga": {"multiple_items_allowed": True}},
+                    "analyst_ids": {"benzinga": {"multiple_items_allowed": True}},
+                    "firm_ids": {"benzinga": {"multiple_items_allowed": True}},
+                    "fields": {"benzinga": {"multiple_items_allowed": True}},
                 },
             )
         )
 
     @exception_handler
     @validate
     def consensus(
@@ -332,15 +332,17 @@
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
@@ -453,15 +455,20 @@
                         ("fmp", "intrinio"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp", "intrinio"]}},
+                info={
+                    "symbol": {
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                    }
+                },
             )
         )
 
     @exception_handler
     @validate
     def forward_sales(
         self,
@@ -576,15 +583,15 @@
                         ("intrinio",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["intrinio"]}},
+                info={"symbol": {"intrinio": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def historical(
         self,
@@ -694,15 +701,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def price_target(
         self,
@@ -850,10 +857,15 @@
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "limit": limit,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["benzinga", "fmp"]}},
+                info={
+                    "symbol": {
+                        "benzinga": {"multiple_items_allowed": True},
+                        "fmp": {"multiple_items_allowed": True},
+                    }
+                },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_fundamental.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_fundamental.py`

 * *Files 1% similar despite different names*

```diff
@@ -1417,16 +1417,16 @@
                     "frequency": frequency,
                     "limit": limit,
                     "tag_type": tag_type,
                     "sort": sort,
                 },
                 extra_params=kwargs,
                 info={
-                    "symbol": {"multiple_items_allowed": ["intrinio"]},
-                    "tag": {"multiple_items_allowed": ["intrinio"]},
+                    "symbol": {"intrinio": {"multiple_items_allowed": True}},
+                    "tag": {"intrinio": {"multiple_items_allowed": True}},
                 },
             )
         )
 
     @exception_handler
     @validate
     def historical_eps(
@@ -2161,16 +2161,16 @@
                 },
                 standard_params={
                     "symbol": symbol,
                     "tag": tag,
                 },
                 extra_params=kwargs,
                 info={
-                    "symbol": {"multiple_items_allowed": ["intrinio"]},
-                    "tag": {"multiple_items_allowed": ["intrinio"]},
+                    "symbol": {"intrinio": {"multiple_items_allowed": True}},
+                    "tag": {"intrinio": {"multiple_items_allowed": True}},
                 },
             )
         )
 
     @exception_handler
     @validate
     def management(
@@ -2347,15 +2347,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def metrics(
         self,
@@ -2666,15 +2666,17 @@
                     "symbol": symbol,
                     "period": period,
                     "limit": limit,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
@@ -2860,15 +2862,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     @deprecated(
         "This endpoint is deprecated; use `/equity/profile` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.3.",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_ownership.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,10 +681,10 @@
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["yfinance"]}},
+                info={"symbol": {"yfinance": {"multiple_items_allowed": True}}},
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_price.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,20 +182,18 @@
                     "interval": interval,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "fmp",
-                            "polygon",
-                            "tiingo",
-                            "yfinance",
-                        ]
+                        "fmp": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "tiingo": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     },
                     "adjusted": {"deprecated": True},
                     "prepost": {"deprecated": True},
                 },
             )
         )
 
@@ -401,15 +399,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def quote(
         self,
@@ -575,12 +573,14 @@
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/equity_shorts.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/equity_shorts.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/etf.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/etf.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def equity_exposure(
         self,
@@ -176,15 +176,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def historical(
         self,
@@ -346,20 +346,18 @@
                     "interval": interval,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "fmp",
-                            "polygon",
-                            "tiingo",
-                            "yfinance",
-                        ]
+                        "fmp": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "tiingo": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     },
                     "adjusted": {"deprecated": True},
                     "prepost": {"deprecated": True},
                 },
             )
         )
 
@@ -801,15 +799,15 @@
                         ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp"]}},
+                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def info(
         self,
@@ -1191,15 +1189,17 @@
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": ["fmp", "intrinio", "yfinance"]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
@@ -1332,15 +1332,20 @@
                         ("fmp", "intrinio"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                 },
                 extra_params=kwargs,
-                info={"symbol": {"multiple_items_allowed": ["fmp", "intrinio"]}},
+                info={
+                    "symbol": {
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                    }
+                },
             )
         )
 
     @exception_handler
     @validate
     def search(
         self,
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_corporate.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_corporate.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,12 +510,12 @@
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                     "category": category,
                 },
                 extra_params=kwargs,
                 info={
-                    "maturity": {"multiple_items_allowed": ["fred"]},
-                    "category": {"multiple_items_allowed": ["fred"]},
+                    "maturity": {"fred": {"multiple_items_allowed": True}},
+                    "category": {"fred": {"multiple_items_allowed": True}},
                 },
             )
         )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_government.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_government.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_rate.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/fixedincome_spreads.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/fixedincome_spreads.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/index.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/index.py`

 * *Files 5% similar despite different names*

```diff
@@ -296,20 +296,18 @@
                     "start_date": start_date,
                     "end_date": end_date,
                     "interval": interval,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "fmp",
-                            "intrinio",
-                            "polygon",
-                            "yfinance",
-                        ]
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @property
     def price(self):
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/openbb/package/news.py` & `openbb_nightly-4.1.7.dev202405100010/openbb/package/news.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,22 +232,20 @@
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
                 },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "multiple_items_allowed": [
-                            "benzinga",
-                            "fmp",
-                            "intrinio",
-                            "polygon",
-                            "tiingo",
-                            "yfinance",
-                        ]
+                        "benzinga": {"multiple_items_allowed": True},
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                        "polygon": {"multiple_items_allowed": True},
+                        "tiingo": {"multiple_items_allowed": True},
+                        "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 class AVEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Alpha Vantage Equity Historical Price Query.
 
     Source: https://www.alphavantage.co/documentation/#time-series-data
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "60m", "1d", "1W", "1M"] = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", ""),
     )
     adjustment: Literal["splits_only", "splits_and_dividends", "unadjusted"] = Field(
         description="The adjustment factor to apply. 'splits_only' is not supported for intraday data.",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/models/historical_eps.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class AlphaVantageHistoricalEpsQueryParams(HistoricalEpsQueryParams):
     """
     AlphaVantage Historical EPS Query Params.
 
     Source: https://www.alphavantage.co/documentation/#earnings
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     period: Literal["annual", "quarter"] = Field(
         default="quarter", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     limit: Optional[int] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/alpha_vantage/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/analyst_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/analyst_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 
     __alias_dict__ = {
         "analyst_ids": "analyst",
         "firm_ids": "firm",
         "limit": "pageSize",
     }
     __json_schema_extra__ = {
-        "analyst_name": ["multiple_items_allowed"],
-        "firm_name": ["multiple_items_allowed"],
-        "analyst_ids": ["multiple_items_allowed"],
-        "firm_ids": ["multiple_items_allowed"],
-        "fields": ["multiple_items_allowed"],
+        "analyst_name": {"multiple_items_allowed": True},
+        "firm_name": {"multiple_items_allowed": True},
+        "analyst_ids": {"multiple_items_allowed": True},
+        "firm_ids": {"multiple_items_allowed": True},
+        "fields": {"multiple_items_allowed": True},
     }
 
     analyst_ids: Optional[str] = Field(
         default=None,
         description="List of analyst IDs to return.",
     )
     firm_ids: Optional[str] = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         "display": "displayOutput",
         "limit": "pageSize",
         "start_date": "dateFrom",
         "end_date": "dateTo",
         "updated_since": "updatedSince",
         "published_since": "publishedSince",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     date: Optional[dateType] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("date", "")
     )
     display: Literal["headline", "abstract", "full"] = Field(
         default="full",
         description="Specify headline only (headline), headline + teaser (abstract), or headline + full body (full).",
@@ -148,18 +148,19 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract data."""
         token = credentials.get("benzinga_api_key") if credentials else ""
 
         base_url = "https://api.benzinga.com/api/v2/news"
 
-        query.sort = f"{query.sort}:{query.order}" if query.sort and query.order else ""
-        querystring = get_querystring(
-            query.model_dump(by_alias=True), ["order", "pageSize"]
+        model = query.model_dump(by_alias=True)
+        model["sort"] = (
+            f"{query.sort}:{query.order}" if query.sort and query.order else ""
         )
+        querystring = get_querystring(model, ["order", "pageSize"])
 
         pages = math.ceil(query.limit / 100) if query.limit else 1
         page_size = 100 if query.limit and query.limit > 100 else query.limit
         urls = [
             f"{base_url}?{querystring}&page={page}&pageSize={page_size}&token={token}"
             for page in range(pages)
         ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/price_target.py` & `openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/price_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-ratings
     """
 
     __alias_dict__ = {
         "limit": "pagesize",
         "symbol": "parameters[tickers]",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=0,
         description="Page offset. For optimization, performance and technical reasons,"
         + " page offsets are limited from 0 - 100000. Limit the query results by other parameters such as date."
         + " Used in conjunction with the limit and date parameters.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/benzinga/openbb_benzinga/models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/benzinga/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/biztoc/openbb_biztoc/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/biztoc/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 class CboeEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """
     Cboe Equity Historical Price Query
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "1d"] = Field(
         default="1d",
         description=(
             QUERY_DESCRIPTIONS.get("interval", "")
             + " The most recent trading day is not including in daily historical data."
             + " Intraday data is only available for the most recent trading day at 1 minute intervals."
@@ -137,15 +137,15 @@
                 if symbol.replace("^", "") in TICKER_EXCEPTIONS
                 or symbol.replace("^", "") in INDEXES.index
                 else base_url + f"/{symbol.replace('^', '')}.json"
             )
             return url
 
         urls = [
-            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])
+            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])  # type: ignore[arg-type]
             for symbol in symbols
         ]
         return await amake_requests(urls, **kwargs)
 
     @staticmethod
     def transform_data(
         query: CboeEquityHistoricalQueryParams, data: List[Dict], **kwargs: Any
@@ -195,14 +195,14 @@
         if len(query.symbol.split(",")) == 1:
             output = output.drop(columns="symbol")
         # Finally, we apply the user-specified date range because it is not filtered at the source.
         output = output[
             (to_datetime(output["date"]) >= to_datetime(query.start_date))
             & (
                 to_datetime(output["date"])
-                <= to_datetime(query.end_date + timedelta(days=1))
+                <= to_datetime(query.end_date + timedelta(days=1))  # type: ignore[operator]
             )
         ]
         return [
             CboeEquityHistoricalData.model_validate(d)
             for d in output.to_dict("records")
         ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_quote.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class CboeEquityQuoteQueryParams(EquityQuoteQueryParams):
     """CBOE Equity Quote Query.
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="When True, the company directories will be cached for"
         + " 24 hours and are used to validate symbols."
         + " The results of the function are not cached. Set as False to bypass.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class CboeIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """CBOE Market Indices Query.
 
     Source: https://www.cboe.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "1d"] = Field(
         default="1d",
         description=(
             QUERY_DESCRIPTIONS.get("interval", "")
             + " The most recent trading day is not including in daily historical data."
             + " Intraday data is only available for the most recent trading day at 1 minute intervals."
@@ -135,28 +135,28 @@
                 url = (
                     base_url + "index_history/"
                     if interval_type == "historical"
                     else base_url + "intraday_chart_data/"
                 )
                 url += f"{symbol.replace('^', '')}.json"
             else:
-                base_url: str = (
+                base_url: str = (  # type: ignore[no-redef]
                     f"https://cdn.cboe.com/api/global/delayed_quotes/charts/{interval_type}"
                 )
                 url = (
                     base_url + f"/_{symbol.replace('^', '')}.json"
                     if symbol.replace("^", "") in TICKER_EXCEPTIONS
                     or symbol.replace("^", "") in INDEXES.index
                     else base_url + f"/{symbol.replace('^', '')}.json"
                 )
 
             return url
 
         urls = [
-            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])
+            _generate_historical_prices_url(symbol, INTERVAL_DICT[query.interval])  # type: ignore[arg-type]
             for symbol in symbols
         ]
 
         return await amake_requests(urls, **kwargs)
 
     # pylint: disable=unused-argument
     @staticmethod
@@ -201,13 +201,13 @@
         if len(query.symbol.split(",")) == 1:
             output = output.drop(columns="symbol")
         # Finally, we apply the user-specified date range because it is not filtered at the source.
         output = output[
             (to_datetime(output["date"]) >= to_datetime(query.start_date))
             & (
                 to_datetime(output["date"])
-                <= to_datetime(query.end_date + timedelta(days=1))
+                <= to_datetime(query.end_date + timedelta(days=1))  # type: ignore[operator]
             )
         ]
         return [
             CboeIndexHistoricalData.model_validate(d) for d in output.to_dict("records")
         ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/cboe/openbb_cboe/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/cboe/openbb_cboe/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/balance_of_payments.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/currency_reference_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/models/eu_yield_curve.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/bps_series.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/ecb_helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/ecb/openbb_ecb/utils/yield_curve_series.py` & `openbb_nightly-4.1.7.dev202405100010/providers/ecb/openbb_ecb/utils/yield_curve_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/available_indicators.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/country_profile.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/country_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pandas import DataFrame, concat
 from pydantic import Field, field_validator
 
 
 class EconDbCountryProfileQueryParams(CountryProfileQueryParams):
     """Country Profile Query."""
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
     latest: bool = Field(
         default=True,
         description="If True, return only the latest data."
         + " If False, return all available data for each indicator.",
     )
     use_cache: bool = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/models/economic_indicators.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/models/economic_indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 INDICATORS = list(helpers.INDICATORS_DESCRIPTIONS)
 
 
 class EconDbEconomicIndicatorsQueryParams(EconomicIndicatorsQueryParams):
     """EconDB Economic Indicators Query."""
 
     __json_schema_extra__ = {
-        "symbol": ["multiple_items_allowed"],
-        "country": ["multiple_items_allowed"],
+        "symbol": {"multiple_items_allowed": True},
+        "country": {"multiple_items_allowed": True},
     }
 
     transform: Union[None, Literal["toya", "tpop", "tusd", "tpgp"]] = Field(
         default=None,
         description="The transformation to apply to the data, default is None."
         + "\n"
         + "\n    tpop: Change from previous period"
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/indicator_countries.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/indicator_countries.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/indicators_descriptions.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/indicators_descriptions.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/main_indicators.py` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/main_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/multipliers.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/multipliers.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/scales.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/scales.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/symbol_to_indicator.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/econdb/openbb_econdb/utils/units.json` & `openbb_nightly-4.1.7.dev202405100010/providers/econdb/openbb_econdb/utils/units.json`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py` & `openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/federal_reserve/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/models/equity_short_interest.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/models/otc_aggregate.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/utils/data_storage.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finra/openbb_finra/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finra/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/compare_groups.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/equity_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class FinvizEquityProfileQueryParams(EquityInfoQueryParams):
     """
     Finviz Equity Profile Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizEquityProfileData(EquityInfoData):
     """Finviz Equity Profile Data."""
 
     __alias_dict__ = {
         "stock_exchange": "exchange",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/key_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class FinvizKeyMetricsQueryParams(KeyMetricsQueryParams):
     """
     Finviz Key Metrics Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizKeyMetricsData(KeyMetricsData):
     """Finviz Key Metrics Data."""
 
     foward_pe: Optional[float] = Field(
         default=None, description="Forward price-to-earnings ratio (forward P/E)"
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/price_performance.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class FinvizPricePerformanceQueryParams(RecentPerformanceQueryParams):
     """
     Finviz Price Performance Query.
 
     Source: https://finviz.com/screener.ashx
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizPricePerformanceData(RecentPerformanceData):
     """Finviz Price Performance Data."""
 
     __alias_dict__ = {
         "symbol": "Ticker",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/models/price_target.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/models/price_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class FinvizPriceTargetQueryParams(PriceTargetQueryParams):
     """Finviz Price Target Query.
 
     Source: https://finviz.com/quote.ashx?
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FinvizPriceTargetData(PriceTargetData):
     """Finviz Price Target Data."""
 
     __alias_dict__ = {
         "published_date": "Date",
@@ -63,20 +63,20 @@
     def extract_data(
         query: FinvizPriceTargetQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Finviz endpoint."""
 
-        results = []
+        results: List[dict] = []
 
         def get_one(symbol) -> List[Dict]:
             """Get the data for one symbol."""
             price_targets = DataFrame()
-            result = []
+            result: List[dict] = []
             try:
                 data = finvizfinance(symbol)
                 price_targets = data.ticker_outer_ratings()
                 if price_targets is None or len(price_targets) == 0:
                     _warn(f"Failed to get data for {symbol}")
                     return result
                 price_targets["symbol"] = symbol
@@ -96,15 +96,15 @@
                 price_targets = price_targets.replace("", None).drop(columns="Price")
             except Exception as e:  # pylint: disable=W0718
                 _warn(f"Failed to get data for {symbol} -> {e}")
                 return result
             result = price_targets.to_dict(orient="records")
             return result
 
-        symbols = query.symbol.split(",")
+        symbols = query.symbol.split(",") if query.symbol else []
         for symbol in symbols:
             result = get_one(symbol)
             if result is not None and result != []:
                 results.extend(result)
 
         return results
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/finviz/openbb_finviz/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405100010/providers/finviz/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/analyst_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/analyst_estimates.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class FMPAnalystEstimatesQueryParams(AnalystEstimatesQueryParams):
     """FMP Analyst Estimates Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/analyst-estimates-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     period: Literal["quarter", "annual"] = Field(
         default="annual", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     limit: Optional[int] = Field(
         default=None, description=QUERY_DESCRIPTIONS.get("limit", "")
     )
@@ -56,15 +56,15 @@
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         symbols = query.symbol.split(",")  # type: ignore
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = create_url(
                 3, f"analyst-estimates/{symbol}", api_key, query, ["symbol"]
             )
             result = await amake_request(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/balance_sheet_growth.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/calendar_splits.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/cash_flow_growth.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_news.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class FMPCompanyNewsQueryParams(CompanyNewsQueryParams):
     """FMP Company News Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/stock-news-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=0,
         description="Page number of the results. Use in combination with limit.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/company_overview.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     FMP Crypto Historical Price Query.
 
     Source:
     https://site.financialmodelingprep.com/developer/docs/cryptocurrency-historical-data-api/#Historical-Daily-Prices
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPCryptoHistoricalData(CryptoHistoricalData):
@@ -96,15 +96,15 @@
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
-                url = f"{base_url}/historical-price-full/crypto/{url_params}"
+                url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
         symbols = query.symbol.split(",")
 
         results = []
         messages = []
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/crypto_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/currency_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """FMP Currency Historical Price Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Historical-Forex-Price
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPCurrencyHistoricalData(CurrencyHistoricalData):
@@ -94,29 +94,26 @@
         base_url = "https://financialmodelingprep.com/api/v3"
         query_str = get_querystring(query.model_dump(), ["symbol"])
 
         def get_url_params(symbol: str) -> str:
             url_params = f"{symbol}?{query_str}&apikey={api_key}"
             url = f"{base_url}/historical-chart/{interval}/{url_params}"
             if interval == "1day":
-                url = f"{base_url}/historical-price-full/forex/{url_params}"
+                url = f"{base_url}/historical-price-full/{url_params}"
             return url
 
         symbols = query.symbol.split(",")
 
         results = []
         messages = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
-
             url = get_url_params(symbol)
-
             data = []
-
             response = await amake_request(url, **kwargs)
 
             if isinstance(response, dict) and response.get("Error Message"):
                 message = f"Error fetching data for {symbol}: {response.get('Error Message', '')}"
                 warn(message)
                 messages.append(message)
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/currency_pairs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,84 @@
-"""FMP Currency Available Pairs Model."""
+"""Intrinio Currency Available Pairs Model."""
 
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_pairs import (
     CurrencyPairsData,
     CurrencyPairsQueryParams,
 )
-from openbb_fmp.utils.helpers import get_data_many
+from openbb_core.provider.utils.errors import EmptyDataError
+from openbb_intrinio.utils.helpers import get_data_many
+from pandas import DataFrame
 from pydantic import Field
 
 
-class FMPCurrencyPairsQueryParams(CurrencyPairsQueryParams):
-    """FMP Currency Available Pairs Query.
+class IntrinioCurrencyPairsQueryParams(CurrencyPairsQueryParams):
+    """Intrinio Currency Available Pairs Query.
 
-    Source: http://site.financialmodelingprep.com/developer/docs/stock-ticker-symbol-lookup-api/?direct=true
+    Source: https://docs.intrinio.com/documentation/web_api/get_forex_pairs_v2
     """
 
 
-class FMPCurrencyPairsData(CurrencyPairsData):
-    """FMP Currency Available Pairs Data."""
+class IntrinioCurrencyPairsData(CurrencyPairsData):
+    """Intrinio Currency Available Pairs Data."""
 
-    symbol: str = Field(description="Symbol of the currency pair.")
-    currency: str = Field(description="Base currency of the currency pair.")
-    stock_exchange: Optional[str] = Field(
-        default=None, description="Stock exchange of the currency pair."
+    __alias_dict__ = {"symbol": "code"}
+
+    base_currency: str = Field(
+        description="ISO 4217 currency code of the base currency."
     )
-    exchange_short_name: Optional[str] = Field(
-        default=None,
-        description="Short name of the stock exchange of the currency pair.",
+    quote_currency: str = Field(
+        description="ISO 4217 currency code of the quote currency."
     )
 
 
-class FMPCurrencyPairsFetcher(
+class IntrinioCurrencyPairsFetcher(
     Fetcher[
-        FMPCurrencyPairsQueryParams,
-        List[FMPCurrencyPairsData],
+        IntrinioCurrencyPairsQueryParams,
+        List[IntrinioCurrencyPairsData],
     ]
 ):
-    """Transform the query, extract and transform the data from the FMP endpoints."""
+    """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> FMPCurrencyPairsQueryParams:
+    def transform_query(params: Dict[str, Any]) -> IntrinioCurrencyPairsQueryParams:
         """Transform the query params."""
-        return FMPCurrencyPairsQueryParams(**params)
+        return IntrinioCurrencyPairsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: FMPCurrencyPairsQueryParams,
+        query: IntrinioCurrencyPairsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
-        """Return the raw data from the FMP endpoint."""
-        api_key = credentials.get("fmp_api_key") if credentials else ""
-
-        base_url = "https://financialmodelingprep.com/api/v3"
-        url = f"{base_url}/symbol/available-forex-currency-pairs?apikey={api_key}"
+        """Return the raw data from the Intrinio endpoint."""
+        api_key = credentials.get("intrinio_api_key") if credentials else ""
 
-        return await get_data_many(url, **kwargs)
+        base_url = "https://api-v2.intrinio.com"
+        url = f"{base_url}/forex/pairs?api_key={api_key}"
+        return await get_data_many(url, "pairs", **kwargs)
 
     @staticmethod
     def transform_data(
-        query: FMPCurrencyPairsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[FMPCurrencyPairsData]:
+        query: IntrinioCurrencyPairsQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[IntrinioCurrencyPairsData]:
         """Return the transformed data."""
-        return [FMPCurrencyPairsData.model_validate(d) for d in data]
+        if not data:
+            raise EmptyDataError("The request was returned empty.")
+        df = DataFrame(data)
+        if query.query:
+            df = df[
+                df["code"].str.contains(query.query, case=False)
+                | df["base_currency"].str.contains(query.query, case=False)
+                | df["quote_currency"].str.contains(query.query, case=False)
+            ]
+        if len(df) == 0:
+            raise EmptyDataError(
+                f"No results were found with the query supplied. -> {query.query}"
+                + " Hint: Names and descriptions are not searchable from Intrinio, try 3-letter symbols."
+            )
+        return [
+            IntrinioCurrencyPairsData.model_validate(d)
+            for d in df.to_dict(orient="records")
+        ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/currency_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPCurrencySnapshotsQueryParams(CurrencySnapshotsQueryParams):
     """FMP Currency Snapshots Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs#exchange-prices-quote
     """
 
-    __json_schema_extra__ = {"base": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"base": {"multiple_items_allowed": True}}
 
 
 class FMPCurrencySnapshotsData(CurrencySnapshotsData):
     """FMP Currency Snapshots Data."""
 
     __alias_dict__ = {
         "last_rate": "price",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/discovery_filings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/earnings_call_transcript.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """FMP Equity Historical Price Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPEquityHistoricalData(EquityHistoricalData):
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_peers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class FMPEquityProfileQueryParams(EquityInfoQueryParams):
     """FMP Equity Profile Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/companies-key-stats-free-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityProfileData(EquityInfoData):
     """FMP Equity Profile Data."""
 
     __alias_dict__ = {
         "name": "companyName",
@@ -44,15 +44,15 @@
         "hq_country": "country",
         "business_phone_no": "phone",
         "industry_category": "industry",
         "employees": "fullTimeEmployees",
         "long_description": "description",
         "first_stock_price_date": "ipoDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     is_etf: bool = Field(description="If the symbol is an ETF.")
     is_actively_trading: bool = Field(description="If the company is actively trading.")
     is_adr: bool = Field(description="If the stock is an ADR.")
     is_fund: bool = Field(description="If the company is a fund.")
     image: Optional[str] = Field(default=None, description="Image of the company.")
     currency: Optional[str] = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class FMPEquityQuoteQueryParams(EquityQuoteQueryParams):
     """FMP Equity Quote Query.
 
     Source: https://financialmodelingprep.com/developer/docs/#Stock-Historical-Price
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityQuoteData(EquityQuoteData):
     """FMP Equity Quote Data."""
 
     __alias_dict__ = {
         "price_avg50": "priceAvg50",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_screener.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class FMPEquityValuationMultiplesQueryParams(EquityValuationMultiplesQueryParams):
     """FMP Equity Valuation Multiples Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Company-Key-Metrics
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEquityValuationMultiplesData(EquityValuationMultiplesData):
     """FMP Equity Valuation Multiples Data."""
 
     __alias_dict__ = {
         "revenue_per_share_ttm": "revenuePerShareTTM",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_fmp.utils.helpers import create_url, response_callback
 from pandas import DataFrame
 
 
 class FMPEtfCountriesQueryParams(EtfCountriesQueryParams):
     """FMP ETF Countries Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfCountriesData(EtfCountriesData):
     """FMP ETF Countries Data."""
 
 
 class FMPEtfCountriesFetcher(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_equity_exposure.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_equity_exposure.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class FMPEtfEquityExposureQueryParams(EtfEquityExposureQueryParams):
     """
     FMP ETF Equity Exposure Query Params.
 
     Source: https://site.financialmodelingprep.com/developer/docs/etf-stock-exposure-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfEquityExposureData(EtfEquityExposureData):
     """FMP ETF Equity Exposure Data."""
 
     __alias_dict__ = {
         "equity_symbol": "assetExposure",
@@ -60,15 +60,15 @@
         query: FMPEtfEquityExposureQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         symbols = query.symbol.split(",")
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get one symbol."""
             url = f"https://financialmodelingprep.com/api/v3/etf-stock-exposure/{symbol}?apikey={api_key}"
             response = await amake_request(
                 url, response_callback=response_callback, **kwargs
             )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings_date.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_holdings_performance.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_holdings_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_core.provider.utils.helpers import amake_request
 from pydantic import Field
 
 
 class FMPEtfInfoQueryParams(EtfInfoQueryParams):
     """FMP ETF Info Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPEtfInfoData(EtfInfoData):
     """FMP ETF Info Data."""
 
     issuer: Optional[str] = Field(
         default=None, description="Company of the ETF.", alias="etfCompany"
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/executive_compensation.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/executive_compensation.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPExecutiveCompensationQueryParams(ExecutiveCompensationQueryParams):
     """FMP Executive Compensation Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/executive-compensation-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     year: Optional[int] = Field(default=None, description="Year of the compensation.")
 
 
 class FMPExecutiveCompensationData(ExecutiveCompensationData):
     """FMP Executive Compensation Data."""
 
@@ -82,15 +82,15 @@
 
         api_key = credentials.get("fmp_api_key") if credentials else ""
 
         base_url = "https://financialmodelingprep.com/api/v4/"
 
         symbols = query.symbol.split(",")
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
 
             url = f"{base_url}/governance/executive_compensation?symbol={symbol}&apikey={api_key}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/forward_eps_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class FMPForwardEpsEstimatesQueryParams(ForwardEpsEstimatesQueryParams):
     """FMP Forward EPS Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/analyst-estimates-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     __alias_dict__ = {"fiscal_period": "period"}
 
     fiscal_period: Literal["annual", "quarter"] = Field(
         default="annual",
         description="The future fiscal period to retrieve estimates for.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_employees.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_eps.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/historical_splits.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/income_statement_growth.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/index_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 class FMPIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """FMP Index Historical Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/historical-index-price-api/
     """
 
     __alias_dict__ = {"start_date": "from", "end_date": "to"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
 
 
 class FMPIndexHistoricalData(IndexHistoricalData):
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/key_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class FMPKeyMetricsQueryParams(KeyMetricsQueryParams):
     """FMP Key Metrics Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/company-key-metrics-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     with_ttm: Optional[bool] = Field(
         default=False, description="Include trailing twelve months (TTM) data."
     )
 
 
 class FMPKeyMetricsData(KeyMetricsData):
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_performance.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class FMPPricePerformanceQueryParams(RecentPerformanceQueryParams):
     """FMP Price Performance Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/stock-split-calendar-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class FMPPricePerformanceData(RecentPerformanceData):
     """FMP Price Performance Data."""
 
     symbol: str = Field(description="The ticker symbol.")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_target.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 class FMPPriceTargetQueryParams(PriceTargetQueryParams):
     """FMP Price Target Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Price-Target
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     with_grade: bool = Field(
         False,
         description="Include upgrades and downgrades in the response.",
     )
 
 
@@ -85,15 +85,15 @@
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         endpoint = "upgrades-downgrades" if query.with_grade else "price-target"
 
         symbols = query.symbol.split(",")  # type: ignore
 
-        results = []
+        results: List[dict] = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
             url = create_url(4, endpoint, api_key, query, exclude=["limit", "symbol"])
             url += f"&symbol={symbol}"
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/price_target_consensus.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 class FMPPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """FMP Price Target Consensus Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/price-target-consensus-api/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for FMP.")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/revenue_business_line.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/revenue_geographic.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/risk_premium.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/treasury_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fmp/openbb_fmp/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fmp/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ameribor_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/cp.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/cpi.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from openbb_fred.utils.fred_base import Fred
 from openbb_fred.utils.fred_helpers import all_cpi_options
 
 
 class FREDConsumerPriceIndexQueryParams(ConsumerPriceIndexQueryParams):
     """FRED Consumer Price Index Query."""
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
 
 class FREDConsumerPriceIndexData(ConsumerPriceIndexData):
     """FRED Consumer Price Index Data."""
 
 
 class FREDConsumerPriceIndexFetcher(
@@ -71,12 +71,11 @@
                 # If the date is not in the dictionary, add it
                 if item["date"] not in transformed_data:
                     transformed_data[item["date"]] = {"date": item["date"]}
                 # Update the dictionary with the country's value data
                 transformed_data[item["date"]].update({country: item["value"]})
 
         # Convert the dictionary to a list of dictionaries
-        transformed_data = list(transformed_data.values())
-
         return [
-            FREDConsumerPriceIndexData.model_validate(item) for item in transformed_data
+            FREDConsumerPriceIndexData.model_validate(item)
+            for item in list(transformed_data.values())
         ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/dwpcr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ecb_interest_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/estr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/fed_projections.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/fed_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ffrmc.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/hqm.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/ice_bofa.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/iorb_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/moody.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/regional.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/series.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     __alias_dict__ = {
         "symbol": "series_id",
         "start_date": "observation_start",
         "end_date": "observation_end",
         "transform": "units",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     frequency: Optional[
         Literal[
             "a",
             "q",
             "m",
             "w",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/sofr_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/sonia_rates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/spot.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/spot.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pydantic import field_validator
 
 
 class FREDSpotRateQueryParams(SpotRateQueryParams):
     """FRED Spot Rate Query."""
 
     __json_schema_extra__ = {
-        "maturity": ["multiple_items_allowed"],
-        "category": ["multiple_items_allowed"],
+        "maturity": {"multiple_items_allowed": True},
+        "category": {"multiple_items_allowed": True},
     }
 
 
 class FREDSpotRateData(SpotRateData):
     """FRED Spot Rate Data."""
 
     __alias_dict__ = {"rate": "value"}
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/tbffr.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/tmc.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/models/us_yield_curve.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/commercial_paper.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/cpi.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/fred_base.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/fred_helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/fred_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/harmonized_cpi.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/fred/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/fred/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/models/treasury_auctions.py` & `openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/government_us/openbb_government_us/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/government_us/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Source: https://docs.intrinio.com/documentation/web_api/get_company_news_v2
     """
 
     __alias_dict__ = {
         "limit": "page_size",
         "source": "specific_source",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     source: Optional[
         Literal["yahoo", "moody", "moody_us_news", "moody_us_press_releases"]
     ] = Field(
         default=None,
         description="The source of the news article.",
     )
@@ -178,29 +178,31 @@
         base_url = "https://api-v2.intrinio.com/companies"
         ignore = (
             ["symbol", "page_size", "is_spam"]
             if not query.source or query.source == "yahoo"
             else ["symbol", "page_size"]
         )
         query_str = get_querystring(query.model_dump(by_alias=True), ignore)
-        symbols = query.symbol.split(",")
+        symbols = query.symbol.split(",") if query.symbol else []
         news: List = []
 
         async def callback(response, session):
             """Response callback."""
             result = await response.json()
             if "error" in result:
                 raise RuntimeError(f"Intrinio Error Message -> {result['error']}")
             symbol = response.url.parts[-2]
             _data = result.get("news", [])
             data = []
             data.extend([{"symbol": symbol, **d} for d in _data])
             articles = len(data)
             next_page = result.get("next_page")
-            while next_page and query.limit > articles:
+            # query.limit can be None...
+            limit = query.limit or 2500
+            while next_page and limit > articles:
                 url = f"{base_url}/{symbol}/news?{query_str}&api_key={api_key}&next_page={next_page}"
                 result = await get_data(url, session=session, **kwargs)
                 _data = result.get("news", [])
                 if _data:
                     data.extend([{"symbol": symbol, **d} for d in _data])
                     articles = len(data)
                 next_page = result.get("next_page")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/financial_attributes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,78 @@
-"""Intrinio Currency Available Pairs Model."""
+"""Intrinio Financial Attributes Model."""
 
+from datetime import datetime
 from typing import Any, Dict, List, Optional
 
+from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.currency_pairs import (
-    CurrencyPairsData,
-    CurrencyPairsQueryParams,
+from openbb_core.provider.standard_models.financial_attributes import (
+    FinancialAttributesData,
+    FinancialAttributesQueryParams,
 )
+from openbb_core.provider.utils.helpers import get_querystring
 from openbb_intrinio.utils.helpers import get_data_many
-from pydantic import Field
 
 
-class IntrinioCurrencyPairsQueryParams(CurrencyPairsQueryParams):
-    """Intrinio Currency Available Pairs Query.
+class IntrinioFinancialAttributesQueryParams(FinancialAttributesQueryParams):
+    """Intrinio Financial Attributes Query."""
 
-    Source: https://docs.intrinio.com/documentation/web_api/get_forex_pairs_v2
-    """
+    __alias_dict__ = {"sort": "sort_order", "limit": "page_size"}
 
 
-class IntrinioCurrencyPairsData(CurrencyPairsData):
-    """Intrinio Currency Available Pairs Data."""
+class IntrinioFinancialAttributesData(FinancialAttributesData):
+    """Intrinio Financial Attributes Data."""
 
-    __alias_dict__ = {"name": "code"}
 
-    code: str = Field(description="Code of the currency pair.", alias="name")
-    base_currency: str = Field(
-        description="ISO 4217 currency code of the base currency."
-    )
-    quote_currency: str = Field(
-        description="ISO 4217 currency code of the quote currency."
-    )
-
-
-class IntrinioCurrencyPairsFetcher(
+class IntrinioFinancialAttributesFetcher(
     Fetcher[
-        IntrinioCurrencyPairsQueryParams,
-        List[IntrinioCurrencyPairsData],
+        IntrinioFinancialAttributesQueryParams,
+        List[IntrinioFinancialAttributesData],
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> IntrinioCurrencyPairsQueryParams:
+    def transform_query(
+        params: Dict[str, Any]
+    ) -> IntrinioFinancialAttributesQueryParams:
         """Transform the query params."""
-        return IntrinioCurrencyPairsQueryParams(**params)
+        transformed_params = params
+
+        now = datetime.now().date()
+        if params.get("start_date") is None:
+            transformed_params["start_date"] = now - relativedelta(years=5)
+
+        if params.get("end_date") is None:
+            transformed_params["end_date"] = now
+
+        return IntrinioFinancialAttributesQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioCurrencyPairsQueryParams,
+        query: IntrinioFinancialAttributesQueryParams,  # pylint: disable=unused-argument
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
+        frequency = "yearly" if query.period == "annual" else "quarterly"
+        data: List[Dict] = []
 
         base_url = "https://api-v2.intrinio.com"
-        url = f"{base_url}/forex/pairs?api_key={api_key}"
+        query_str = get_querystring(query.model_dump(by_alias=True), ["frequency"])
+        query_str = f"{query_str}&frequency={frequency}"
+
+        url = f"{base_url}/historical_data/{query.symbol}/{query.tag}?{query_str}&api_key={api_key}"
+        # data = get_data_one(url).get("historical_data", [])
+        data = await get_data_many(url, "historical_data")
 
-        return await get_data_many(url, "pairs", **kwargs)
+        return data
 
     @staticmethod
     def transform_data(
-        query: IntrinioCurrencyPairsQueryParams, data: List[Dict], **kwargs: Any
-    ) -> List[IntrinioCurrencyPairsData]:
+        query: IntrinioFinancialAttributesQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
+    ) -> List[IntrinioFinancialAttributesData]:
         """Return the transformed data."""
-        return [IntrinioCurrencyPairsData.model_validate(d) for d in data]
+        return [IntrinioFinancialAttributesData.model_validate(item) for item in data]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_info.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class IntrinioEquityInfoQueryParams(EquityInfoQueryParams):
     """Intrinio Equity Info Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_company_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioEquityInfoData(EquityInfoData):
     """Intrinio Equity Info Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Intrinio Equity Quote Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_security_realtime_price_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     symbol: str = Field(
         description="A Security identifier (Ticker, FIGI, ISIN, CUSIP, Intrinio ID)."
     )
     source: SOURCES = Field(default="iex", description="Source of the data.")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class IntrinioEtfInfoQueryParams(EtfInfoQueryParams):
     """
     Intrinio ETF Info Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioEtfInfoData(EtfInfoData):
     """Intrinio ETF Info Data."""
 
     __alias_dict__ = {
         "symbol": "ticker",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_price_performance.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_price_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
     Intrinio ETF Performance Query Params.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_stats_v2
     Source: https://docs.intrinio.com/documentation/web_api/get_etf_analytics_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     return_type: Literal["trailing", "calendar"] = Field(
         default="trailing",
         description="The type of returns to return, a trailing or calendar window.",
     )
     adjustment: Literal["splits_only", "splits_and_dividends"] = Field(
         default="splits_and_dividends",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/financial_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/search_attributes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,73 @@
-"""Intrinio Financial Attributes Model."""
+"""Intrinio Search Attributes Model."""
 
-from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from dateutil.relativedelta import relativedelta
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_core.provider.standard_models.financial_attributes import (
-    FinancialAttributesData,
-    FinancialAttributesQueryParams,
+from openbb_core.provider.standard_models.search_attributes import (
+    SearchAttributesData,
+    SearchAttributesQueryParams,
 )
 from openbb_core.provider.utils.helpers import get_querystring
-from openbb_intrinio.utils.helpers import get_data_many
+from openbb_intrinio.utils.helpers import get_data_one
 
 
-class IntrinioFinancialAttributesQueryParams(FinancialAttributesQueryParams):
-    """Intrinio Financial Attributes Query."""
+class IntrinioSearchAttributesQueryParams(SearchAttributesQueryParams):
+    """Intrinio Search Attributes Query.
 
-    __alias_dict__ = {"sort": "sort_order", "limit": "page_size"}
+    Source: https://docs.intrinio.com/documentation/web_api/search_data_tags_v2
+    """
 
+    __alias_dict__ = {"limit": "page_size"}
 
-class IntrinioFinancialAttributesData(FinancialAttributesData):
-    """Intrinio Financial Attributes Data."""
 
+class IntrinioSearchAttributesData(SearchAttributesData):
+    """Intrinio Search Attributes Data."""
 
-class IntrinioFinancialAttributesFetcher(
+    __alias_dict__ = {
+        "parent_name": "parent",
+        "transaction": "balance",
+    }
+
+
+class IntrinioSearchAttributesFetcher(
     Fetcher[
-        IntrinioFinancialAttributesQueryParams,
-        List[IntrinioFinancialAttributesData],
+        IntrinioSearchAttributesQueryParams,
+        List[IntrinioSearchAttributesData],
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
-    def transform_query(
-        params: Dict[str, Any]
-    ) -> IntrinioFinancialAttributesQueryParams:
+    def transform_query(params: Dict[str, Any]) -> IntrinioSearchAttributesQueryParams:
         """Transform the query params."""
-        transformed_params = params
-
-        now = datetime.now().date()
-        if params.get("start_date") is None:
-            transformed_params["start_date"] = now - relativedelta(years=5)
-
-        if params.get("end_date") is None:
-            transformed_params["end_date"] = now
-
-        return IntrinioFinancialAttributesQueryParams(**transformed_params)
+        return IntrinioSearchAttributesQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: IntrinioFinancialAttributesQueryParams,  # pylint: disable=unused-argument
+        query: IntrinioSearchAttributesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Intrinio endpoint."""
         api_key = credentials.get("intrinio_api_key") if credentials else ""
-        frequency = "yearly" if query.period == "annual" else "quarterly"
-        data: List[Dict] = []
 
         base_url = "https://api-v2.intrinio.com"
-        query_str = get_querystring(query.model_dump(by_alias=True), ["frequency"])
-        query_str = f"{query_str}&frequency={frequency}"
+        query_str = get_querystring(query.model_dump(by_alias=True), [])
+
+        url = f"{base_url}/data_tags/search?{query_str}&api_key={api_key}"
+        data = await get_data_one(url, **kwargs)
 
-        url = f"{base_url}/historical_data/{query.symbol}/{query.tag}?{query_str}&api_key={api_key}"
-        # data = get_data_one(url).get("historical_data", [])
-        data = await get_data_many(url, "historical_data")
+        # Intrinio doesn't return the correct number of results when using the limit parameter
+        # Temporary fix until they fix it
+        data = data.get("tags", [])[: query.limit]
 
         return data
 
     @staticmethod
     def transform_data(
-        query: IntrinioFinancialAttributesQueryParams,
+        query: IntrinioSearchAttributesQueryParams,
         data: List[Dict],
         **kwargs: Any,
-    ) -> List[IntrinioFinancialAttributesData]:
+    ) -> List[IntrinioSearchAttributesData]:
         """Return the transformed data."""
-        return [IntrinioFinancialAttributesData.model_validate(item) for item in data]
+        return [IntrinioSearchAttributesData.model_validate(item) for item in data]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/financial_ratios.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioForwardEpsEstimatesQueryParams(ForwardEpsEstimatesQueryParams):
     """Intrinio Forward EPS Estimates Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales_estimates_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     fiscal_year: Optional[int] = Field(
         default=None,
         description="The future fiscal year to retrieve estimates for."
         + " When no symbol and year is supplied the current calendar year is used.",
     )
     fiscal_period: Union[Literal["fy", "q1", "q2", "q3", "q4"], None] = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioForwardSalesEstimatesQueryParams(ForwardSalesEstimatesQueryParams):
     """Intrinio Forward Sales Estimates Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales_estimates_v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     fiscal_year: Optional[int] = Field(
         default=None,
         description="The future fiscal year to retrieve estimates for."
         + " When no symbol and year is supplied the current calendar year is used.",
     )
     fiscal_period: Union[Literal["fy", "q1", "q2", "q3", "q4"], None] = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/fred_series.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/historical_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/historical_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     """Intrinio Historical Attributes Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_historical_data_v2
     """
 
     __alias_dict__ = {"sort": "sort_order", "limit": "page_size", "tag_type": "type"}
     __json_schema_extra__ = {
-        "tag": ["multiple_items_allowed"],
-        "symbol": ["multiple_items_allowed"],
+        "tag": {"multiple_items_allowed": True},
+        "symbol": {"multiple_items_allowed": True},
     }
 
 
 class IntrinioHistoricalAttributesData(HistoricalAttributesData):
     """Intrinio Historical Attributes Data."""
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/index_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Intrinio Index Historical Query.
 
     Source:
     https://docs.intrinio.com/documentation/web_api/get_stock_market_index_historical_data_v2
     """
 
     __alias_dict__ = {"limit": "page_size", "sort": "sort_order"}
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     limit: Optional[int] = Field(
         default=10000,
         description=QUERY_DESCRIPTIONS.get("limit", ""),
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/institutional_ownership.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/key_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 class IntrinioKeyMetricsQueryParams(KeyMetricsQueryParams):
     """
     Intrinio Key Metrics Query.
 
     Source: https://data.intrinio.com/data-tags/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class IntrinioKeyMetricsData(KeyMetricsData):
     """Intrinio Key Metrics Data."""
 
     __alias_dict__ = {
         "market_cap": "marketcap",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/latest_attributes.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/latest_attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     """Intrinio Latest Attributes Query.
 
     Source: https://docs.intrinio.com/documentation/web_api/get_data_point_number_v2
             https://docs.intrinio.com/documentation/web_api/get_data_point_text_v2
     """
 
     __json_schema_extra__ = {
-        "tag": ["multiple_items_allowed"],
-        "symbol": ["multiple_items_allowed"],
+        "tag": {"multiple_items_allowed": True},
+        "symbol": {"multiple_items_allowed": True},
     }
 
 
 class IntrinioLatestAttributesData(LatestAttributesData):
     """Intrinio Latest Attributes Data."""
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/options_unusual.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class IntrinioPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """Intrinio Price Target Consensus  Query.
 
     https://docs.intrinio.com/documentation/web_api/get_zacks_sales__v2
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     industry_group_number: Optional[int] = Field(
         default=None,
         description="The Zacks industry group number.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/reported_financials.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/intrinio/openbb_intrinio/utils/references.py` & `openbb_nightly-4.1.7.dev202405100010/providers/intrinio/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/cot.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/cot_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/economic_calendar.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 class NasdaqEconomicCalendarQueryParams(EconomicCalendarQueryParams):
     """Nasdaq Economic Calendar Query.
 
     Source: https://www.nasdaq.com/market-activity/economic-calendar
     """
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
     country: Optional[str] = Field(
         default=None,
         description="Country of the event",
     )
 
     @field_validator("country", mode="before", check_fields=False)
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/historical_dividends.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from openbb_nasdaq.utils.helpers import IPO_HEADERS
 from pydantic import Field, field_validator
 
 
 class NasdaqHistoricalDividendsQueryParams(HistoricalDividendsQueryParams):
     """Nasdaq Historical Dividends Query Params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class NasdaqHistoricalDividendsData(HistoricalDividendsData):
     """Nasdaq Historical Dividends Data."""
 
     __alias_dict__ = {
         "ex_dividend_date": "exOrEffDate",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/models/top_retail.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/query_params.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/nasdaq/openbb_nasdaq/utils/series_ids.py` & `openbb_nightly-4.1.7.dev202405100010/providers/nasdaq/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/composite_leading_indicator.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_forecast.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_nominal.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/gdp_real.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/long_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/short_term_interest_rate.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/models/unemployment.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/utils/constants.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/oecd/openbb_oecd/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/oecd/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/company_news.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class PolygonCompanyNewsQueryParams(CompanyNewsQueryParams):
     """Polygon Company News Query.
 
     Source: https://polygon.io/docs/stocks/get_v2_reference_news
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
     __alias_dict__ = {
         "symbol": "ticker",
         "start_date": "published_utc.gte",
         "end_date": "published_utc.lte",
     }
 
     order: Optional[Literal["asc", "desc"]] = Field(
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/crypto_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class PolygonCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Polygon Crypto Historical Price Query.
 
     Source: https://polygon.io/docs/crypto/get_v2_aggs_ticker__cryptoticker__range__multiplier___timespan___from___to
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class PolygonCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Polygon Currency Historical Price Query.
 
     Source: https://polygon.io/docs/forex/get_v2_aggs_ticker__forexticker__range__multiplier___timespan___from___to
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_pairs.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_pairs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,170 +1,138 @@
 """Polygon Currency Available Pairs Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import (
     date as dateType,
     datetime,
 )
-from typing import Any, Dict, List, Literal, Optional
+from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.currency_pairs import (
     CurrencyPairsData,
     CurrencyPairsQueryParams,
 )
-from openbb_core.provider.utils.descriptions import QUERY_DESCRIPTIONS
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_polygon.utils.helpers import get_data
-from pydantic import Field, PositiveInt, field_validator
+from pandas import DataFrame
+from pydantic import Field, field_validator
 
 
 class PolygonCurrencyPairsQueryParams(CurrencyPairsQueryParams):
     """Polygon Currency Available Pairs Query.
 
     Source: https://polygon.io/docs/forex/get_v3_reference_tickers
     """
 
-    symbol: Optional[str] = Field(
-        default=None, description="Symbol of the pair to search."
-    )
-    date: Optional[dateType] = Field(
-        default=None, description=QUERY_DESCRIPTIONS.get("date", "")
-    )
-    search: Optional[str] = Field(
-        default="",
-        description="Search for terms within the ticker and/or company name.",
-    )
-    active: Optional[bool] = Field(
-        default=True,
-        description="Specify if the tickers returned should be actively traded on the queried date.",
-    )
-    order: Optional[Literal["asc", "desc"]] = Field(
-        default="asc", description="Order data by ascending or descending."
-    )
-    sort: Optional[
-        Literal[
-            "ticker",
-            "name",
-            "market",
-            "locale",
-            "currency_symbol",
-            "currency_name",
-            "base_currency_symbol",
-            "base_currency_name",
-            "last_updated_utc",
-            "delisted_utc",
-        ]
-    ] = Field(default=None, description="Sort field used for ordering.")
-    limit: Optional[PositiveInt] = Field(
-        default=1000, description=QUERY_DESCRIPTIONS.get("limit", "")
-    )
-
 
 class PolygonCurrencyPairsData(CurrencyPairsData):
     """Polygon Currency Available Pairs Data."""
 
-    market: str = Field(description="Name of the trading market. Always 'fx'.")
-    locale: str = Field(description="Locale of the currency pair.")
+    __alias_dict__ = {
+        "last_updated": "last_updated_utc",
+        "delisted": "delisted_utc",
+        "name": "currency_name",
+        "symbol": "ticker",
+    }
     currency_symbol: Optional[str] = Field(
         default=None, description="The symbol of the quote currency."
     )
-    currency_name: Optional[str] = Field(
-        default=None, description="Name of the quote currency."
-    )
     base_currency_symbol: Optional[str] = Field(
         default=None, description="The symbol of the base currency."
     )
     base_currency_name: Optional[str] = Field(
         default=None, description="Name of the base currency."
     )
-    last_updated_utc: datetime = Field(description="The last updated timestamp in UTC.")
-    delisted_utc: Optional[datetime] = Field(
-        default=None, description="The delisted timestamp in UTC."
+    market: str = Field(description="Name of the trading market. Always 'fx'.")
+    locale: str = Field(description="Locale of the currency pair.")
+    last_updated: Optional[dateType] = Field(
+        default=None, description="The date the reference data was last updated."
+    )
+    delisted: Optional[dateType] = Field(
+        default=None, description="The date the item was delisted."
     )
 
-    @field_validator("last_updated_utc", mode="before", check_fields=False)
+    @field_validator("last_updated", "delisted", mode="before", check_fields=False)
     @classmethod
     def last_updated_utc_validate(cls, v):  # pylint: disable=E0213
         """Return the parsed last updated timestamp in UTC."""
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ")
-
-    @field_validator("delisted_utc", mode="before", check_fields=False)
-    @classmethod
-    def delisted_utc_validate(cls, v):  # pylint: disable=E0213
-        """Return the parsed delisted timestamp in UTC."""
-        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ")
+        return datetime.strptime(v, "%Y-%m-%dT%H:%M:%SZ").date() if v else None
 
 
 class PolygonCurrencyPairsFetcher(
     Fetcher[
         PolygonCurrencyPairsQueryParams,
         List[PolygonCurrencyPairsData],
     ]
 ):
-    """Transform the query, extract and transform the data from the Polygon endpoints."""
+    """Polygon Currency Pairs Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> PolygonCurrencyPairsQueryParams:
-        """Transform the query parameters. Ticker is set if symbol is provided."""
-        transform_params = params
-        now = datetime.now().date().isoformat()
-        symbol = params.get("symbol")
-        transform_params["symbol"] = f"ticker=C:{symbol.upper()}" if symbol else ""
-        if params.get("date") is None:
-            transform_params["date"] = now
-
-        return PolygonCurrencyPairsQueryParams(**transform_params)
+        """Transform the query parameters."""
+        return PolygonCurrencyPairsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: PolygonCurrencyPairsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
-    ) -> List[dict]:
+    ) -> List[Dict]:
         """Extract the data from the Polygon API."""
         api_key = credentials.get("polygon_api_key") if credentials else ""
-
         request_url = (
             f"https://api.polygon.io/v3/reference/"
-            f"tickers?{query.symbol}&market=fx&date={query.date}&"
-            f"search={query.search}&active={query.active}&order={query.order}&"
-            f"limit={query.limit}"
+            f"tickers?&market=fx&limit=1000"
+            f"&apiKey={api_key}"
         )
-        if query.sort:
-            request_url += f"&sort={query.sort}"
-        request_url = f"{request_url}&apiKey={api_key}"
         data = {"next_url": request_url}
         all_data: List[Dict] = []
         while "next_url" in data:
             data = await get_data(request_url, **kwargs)
-
             if isinstance(data, list):
                 raise ValueError("Expected a dict, got a list")
-
             if len(data["results"]) == 0:
                 raise RuntimeError(
                     "No results found. Please change your query parameters."
                 )
-
             if data["status"] == "OK":
                 results = data.get("results")
                 if not isinstance(results, list):
                     raise ValueError(
                         "Expected 'results' to be a list, got something else."
                     )
                 all_data.extend(results)
             elif data["status"] == "ERROR":
                 raise UserWarning(data["error"])
-
             if "next_url" in data:
                 request_url = f"{data['next_url']}&apiKey={api_key}"
-
         return all_data
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: PolygonCurrencyPairsQueryParams,
-        data: List[dict],
+        data: List[Dict],
         **kwargs: Any,
     ) -> List[PolygonCurrencyPairsData]:
-        """Transform the data into a list of PolygonCurrencyPairsData."""
-        return [PolygonCurrencyPairsData.model_validate(d) for d in data]
+        """Filter data by search query and validate the model."""
+        if not data:
+            raise EmptyDataError("The request was returned empty.")
+        df = DataFrame(data)
+        df["ticker"] = df["ticker"].str.replace("C:", "")
+        if query.query:
+            df = df[
+                df["name"].str.contains(query.query, case=False)
+                | df["base_currency_name"].str.contains(query.query, case=False)
+                | df["currency_name"].str.contains(query.query, case=False)
+                | df["base_currency_symbol"].str.contains(query.query, case=False)
+                | df["currency_symbol"].str.contains(query.query, case=False)
+                | df["ticker"].str.contains(query.query, case=False)
+            ]
+        if len(df) == 0:
+            raise EmptyDataError(
+                f"No results were found with the query supplied. -> {query.query}"
+            )
+        return [
+            PolygonCurrencyPairsData.model_validate(d) for d in df.to_dict("records")
+        ]
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/currency_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/currency_snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 class PolygonCurrencySnapshotsQueryParams(CurrencySnapshotsQueryParams):
     """Polygon Currency Snapshots Query Parameters.
 
 
     Source: https://polygon.io/docs/forex/get_v2_snapshot_locale_global_markets_forex_tickers
     """
 
-    __json_schema_extra__ = {"base": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"base": {"multiple_items_allowed": True}}
 
 
 class PolygonCurrencySnapshotsData(CurrencySnapshotsData):
     """Polygon Currency Snapshots Data."""
 
     vwap: Optional[float] = Field(
         description="The volume-weighted average price.", default=None
@@ -111,29 +111,29 @@
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data."""
         api_key = credentials.get("polygon_api_key") if credentials else ""
         url = f"https://api.polygon.io/v2/snapshot/locale/global/markets/forex/tickers?apiKey={api_key}"
         results = await amake_request(url, **kwargs)
-        if results.get("status") != "OK":
-            raise RuntimeError(f"Error: {results.get('status')}")
-        return results.get("tickers", [])
+        if results.get("status") != "OK":  # type: ignore[union-attr]
+            raise RuntimeError(f"Error: {results.get('status')}")  # type: ignore[union-attr]
+        return results.get("tickers", [])  # type: ignore[union-attr]
 
     @staticmethod
     def transform_data(  # pylint: disable=too-many-locals, too-many-statements
         query: PolygonCurrencySnapshotsQueryParams,
         data: List[Dict],
         **kwargs: Any,
     ) -> List[PolygonCurrencySnapshotsData]:
         """Transform the data."""
         if not data:
             raise EmptyDataError("No data returned.")
         counter_currencies = (
-            query.counter_currencies.upper().split(",")
+            query.counter_currencies.upper().split(",")  # type: ignore[union-attr]
             if query.counter_currencies
             else []
         )
 
         # Filter the data only for the symbols requested.
         df = DataFrame(data)
         df.ticker = df.ticker.str.replace("C:", "")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 class PolygonEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Polygon Equity Historical Price Query.
 
     Source: https://polygon.io/docs/stocks/getting-started
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/equity_nbbo.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/index_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 class PolygonIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """Polygon Index Historical Query.
 
     Source: https://polygon.io/docs/indices/getting-started
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: str = Field(
         default="1d",
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " The numeric portion of the interval can be any positive integer."
         + " The letter portion can be one of the following: s, m, h, d, W, M, Q, Y",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/models/market_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/polygon/openbb_polygon/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/polygon/openbb_polygon/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/cik_map.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/equity_ftd.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/form_13FHR.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/institutions_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/institutions_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/rss_litigation.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/rss_litigation.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/schema_files.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/schema_files.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/sic_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/sic_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/models/symbol_map.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/models/symbol_map.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/definitions.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/sec/openbb_sec/utils/parse_13f.py` & `openbb_nightly-4.1.7.dev202405100010/providers/sec/openbb_sec/utils/parse_13f.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_nightly-4.1.7.dev202405100010/providers/seeking_alpha/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/stockgrid/openbb_stockgrid/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/stockgrid/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/stockgrid/openbb_stockgrid/models/short_volume.py` & `openbb_nightly-4.1.7.dev202405100010/providers/stockgrid/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     offset: Optional[int] = Field(
         default=0, description="Page offset, used in conjunction with limit."
     )
     source: Optional[str] = Field(
         default=None, description="A comma-separated list of the domains requested."
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
         "interval": "resampleFreq",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     exchanges: Optional[List[str]] = Field(
         default=None,
         description=(
@@ -121,15 +121,15 @@
         """Return the raw data from the Tiingo endpoint."""
         api_key = credentials.get("tiingo_token") if credentials else ""
 
         base_url = "https://api.tiingo.com/tiingo/crypto/prices"
         query_str = get_querystring(
             query.model_dump(by_alias=False), ["tickers", "resampleFreq"]
         )
-        results = []
+        results: List[dict] = []
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             result = await response.json()
             symbol = response.url.query.get("tickers", "")
             if not result:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/currency_historical.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     __alias_dict__ = {
         "symbol": "tickers",
         "start_date": "startDate",
         "end_date": "endDate",
         "interval": "resampleFreq",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "30m", "1h", "4h", "1d"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     _frequency: Literal["daily", "weekly", "monthly", "annually"] = PrivateAttr(
         default=None
     )
@@ -102,15 +102,15 @@
 
         api_key = credentials.get("tiingo_token") if credentials else ""
 
         base_url = "https://api.tiingo.com/tiingo/fx/prices"
         query_str = get_querystring(
             query.model_dump(by_alias=False), ["tickers", "resampleFreq"]
         )
-        results = []
+        results: List[dict] = []
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             result = await response.json()
             symbol = response.url.query.get("tickers", "")
             if not result:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Source: https://www.tiingo.com/documentation/end-of-day
     """
 
     __alias_dict__ = {
         "start_date": "startDate",
         "end_date": "endDate",
     }
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1d", "1W", "1M", "1Y"] = Field(
         default="1d", description=QUERY_DESCRIPTIONS.get("interval", "")
     )
     _frequency: Literal["daily", "weekly", "monthly", "annually"] = PrivateAttr(
         default=None
     )
@@ -138,15 +138,15 @@
         query_str = get_querystring(
             query.model_dump(by_alias=True), ["symbol", "interval"]
         )
 
         async def callback(response: ClientResponse, _: Any) -> List[Dict]:
             data = await response.json()
             symbol = response.url.parts[-2]
-            results = []
+            results: List[dict] = []
             if not data:
                 _warn(f"No data found the the symbol: {symbol}")
                 return results
 
             if isinstance(data, List):
                 results = data
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/models/world_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tiingo/openbb_tiingo/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tiingo/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/bond_prices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/calendar_earnings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/company_filings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/company_news.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxCompanyNewsQueryParams(CompanyNewsQueryParams):
     """TMX Stock News query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=1, description="The page number to start from. Use with limit."
     )
 
     @field_validator("symbol", mode="before")
     @classmethod
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Canadian Depositary Receipts (CDRs) are: "AAPL:AQL"
 
     CDRs are the underlying asset for CAD-hedged assets.
 
     source: https://money.tmx.com
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Union[
         Literal["1m", "2m", "5m", "15m", "30m", "60m", "1h", "1d", "1W", "1M"], str, int
     ] = Field(  # type: ignore
         description=QUERY_DESCRIPTIONS.get("interval", "")
         + " Or, any integer (entered as a string) representing the number of minutes."
         + " Default is daily data."
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, model_validator
 
 
 class TmxEquityProfileQueryParams(EquityInfoQueryParams):
     """TMX Equity Profile query params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TmxEquityProfileData(EquityInfoData):
     """TMX Equity Profile Data."""
 
     __alias_dict__ = {
         "short_description": "shortDescription",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 _warn = warnings.warn
 
 
 class TmxEquityQuoteQueryParams(EquityQuoteQueryParams):
     """TMX Equity Profile query params."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TmxEquityQuoteData(EquityQuoteData):
     """TMX Equity Profile Data."""
 
     __alias_dict__ = {
         "last_price": "price",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_countries.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_countries.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 _warn = warnings.warn
 
 
 class TmxEtfCountriesQueryParams(EtfCountriesQueryParams):
     """TMX ETF Countries Query Params"""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request. All ETF data comes from a single JSON file that is updated daily."
         + " To bypass, set to False. If True, the data will be cached for 4 hours.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_holdings.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from openbb_tmx.utils.helpers import get_all_etfs
 from pydantic import Field, field_validator
 
 
 class TmxEtfInfoQueryParams(EtfInfoQueryParams):
     """TMX ETF Info Query Params"""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     use_cache: bool = Field(
         default=True,
         description="Whether to use a cached request. All ETF data comes from a single JSON file that is updated daily."
         + " To bypass, set to False. If True, the data will be cached for 4 hours.",
     )
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/etf_sectors.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/gainers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_constituents.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_sectors.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/index_snapshots.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/insider_trading.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_tmx.utils.helpers import get_data_from_gql, get_random_agent
 from pydantic import Field, field_validator
 
 
 class TmxPriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """TMX Price Target Consensus Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for TMX.")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/models/treasury_prices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/utils/gql.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tmx/openbb_tmx/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tmx/openbb_tmx/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from pydantic import Field
 from pytz import timezone
 
 
 class TradierEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Tradier Equity Historical Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal["1m", "5m", "15m", "1d", "1W", "1M"] = Field(
         description=QUERY_DESCRIPTIONS.get("interval", ""),
         default="1d",
     )
     extended_hours: bool = Field(
         default=False,
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_quote.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pydantic import Field, field_validator, model_validator
 from pytz import timezone
 
 
 class TradierEquityQuoteQueryParams(EquityQuoteQueryParams):
     """Tradier Equity Quote Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class TradierEquityQuoteData(EquityQuoteData):
     """Tradier Equity Quote Data."""
 
     __alias_dict__ = {
         "name": "description",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/equity_search.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/models/options_chains.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradier/openbb_tradier/utils/constants.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradier/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class TEEconomicCalendarQueryParams(EconomicCalendarQueryParams):
     """Trading Economics Economic Calendar Query.
 
     Source: https://docs.tradingeconomics.com/economic_calendar/
     """
 
-    __json_schema_extra__ = {"country": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"country": {"multiple_items_allowed": True}}
 
     # TODO: Probably want to figure out the list we can use.
     country: Optional[str] = Field(default=None, description="Country of the event.")
     importance: Optional[IMPORTANCE] = Field(
         default=None, description="Importance of the event."
     )
     group: Optional[GROUPS] = Field(default=None, description="Grouping of events")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py` & `openbb_nightly-4.1.7.dev202405100010/providers/tradingeconomics/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/active.py` & `openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/gainers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/wsj/openbb_wsj/models/losers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/wsj/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/__init__.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/active.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/available_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/balance_sheet.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/cash_flow.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/company_news.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/company_news.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class YFinanceCompanyNewsQueryParams(CompanyNewsQueryParams):
     """YFinance Company News Query.
 
     Source: https://finance.yahoo.com/news/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceCompanyNewsData(CompanyNewsData):
     """YFinance Company News Data."""
 
     __alias_dict__ = {
         "symbols": "relatedTickers",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/crypto_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/crypto_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class YFinanceCryptoHistoricalQueryParams(CryptoHistoricalQueryParams):
     """Yahoo Finance Crypto Historical Price Query.
 
     Source: https://finance.yahoo.com/crypto/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/currency_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/currency_historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class YFinanceCurrencyHistoricalQueryParams(CurrencyHistoricalQueryParams):
     """Yahoo Finance Currency Price Query.
 
     Source: https://finance.yahoo.com/currencies/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_historical.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class YFinanceEquityHistoricalQueryParams(EquityHistoricalQueryParams):
     """Yahoo Finance Equity Historical Price Query.
 
     Source: https://finance.yahoo.com/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_profile.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEquityProfileQueryParams(EquityInfoQueryParams):
     """YFinance Equity Profile Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEquityProfileData(EquityInfoData):
     """YFinance Equity Profile Data."""
 
     __alias_dict__ = {
         "name": "longName",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/equity_quote.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEquityQuoteQueryParams(EquityQuoteQueryParams):
     """YFinance Equity Quote Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEquityQuoteData(EquityQuoteData):
     """YFinance Equity Quote Data."""
 
     __alias_dict__ = {
         "name": "longName",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/etf_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/etf_info.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/etf_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceEtfInfoQueryParams(EtfInfoQueryParams):
     """YFinance ETF Info Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceEtfInfoData(EtfInfoData):
     """YFinance ETF Info Data."""
 
     __alias_dict__ = {
         "name": "longName",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/futures_curve.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/futures_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/futures_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 class YFinanceFuturesHistoricalQueryParams(FuturesHistoricalQueryParams):
     """Yahoo Finance Futures historical Price Query.
 
     Source: https://finance.yahoo.com/crypto/
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/gainers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/historical_dividends.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/income_statement.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/index_historical.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/index_historical.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 class YFinanceIndexHistoricalQueryParams(IndexHistoricalQueryParams):
     """YFinance Index Historical Query.
 
     Source: https://finance.yahoo.com/world-indices
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Literal[
         "1m",
         "2m",
         "5m",
         "15m",
         "30m",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/key_executives.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/key_metrics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/key_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceKeyMetricsQueryParams(KeyMetricsQueryParams):
     """YFinance Key Metrics Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceKeyMetricsData(KeyMetricsData):
     """YFinance Key Metrics Data."""
 
     __alias_dict__ = {
         "market_cap": "marketCap",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/losers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/market_indices.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/market_indices.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 class YFinanceMarketIndicesQueryParams(MarketIndicesQueryParams):
     """YFinance Market Indices Query.
 
     Source: https://finance.yahoo.com/world-indices
     """
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     interval: Optional[INTERVALS] = Field(default="1d", description="Data granularity.")
     period: Optional[PERIODS] = Field(
         default="max", description=QUERY_DESCRIPTIONS.get("period", "")
     )
     prepost: bool = Field(default=True, description="Include Pre and Post market data.")
     rounding: bool = Field(default=True, description="Round prices to two decimals?")
@@ -57,15 +57,15 @@
 
         if params.get("start_date") is None:
             transformed_params["start_date"] = now - relativedelta(years=1)
 
         if params.get("end_date") is None:
             transformed_params["end_date"] = now
 
-        tickers = params.get("symbol").lower().split(",")
+        tickers = params.get("symbol", "").lower().split(",")
 
         new_tickers = []
         for ticker in tickers:
             _ticker = ""
             indices = pd.DataFrame(INDICES).transpose().reset_index()
             indices.columns = ["code", "name", "symbol"]
 
@@ -119,15 +119,15 @@
         if query.start_date:
             if "date" in data.columns:
                 data.set_index("date", inplace=True)
                 data.index = to_datetime(data.index)
 
             data = data[
                 (data.index >= to_datetime(query.start_date))
-                & (data.index <= to_datetime(query.end_date + timedelta(days=days)))
+                & (data.index <= to_datetime(query.end_date + timedelta(days=days)))  # type: ignore[operator]
             ]
 
         data.reset_index(inplace=True)
         data.rename(columns={"index": "date"}, inplace=True)
 
         return data.to_dict("records")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/price_target_consensus.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/price_target_consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 _warn = warnings.warn
 
 
 class YFinancePriceTargetConsensusQueryParams(PriceTargetConsensusQueryParams):
     """YFinance Price Target Consensus Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     @field_validator("symbol", mode="before", check_fields=False)
     @classmethod
     def check_symbol(cls, value):
         """Check the symbol."""
         if not value:
             raise RuntimeError("Error: Symbol is a required field for yFinance.")
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/share_statistics.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/share_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 _warn = warnings.warn
 
 
 class YFinanceShareStatisticsQueryParams(ShareStatisticsQueryParams):
     """YFinance Share Statistics Query."""
 
-    __json_schema_extra__ = {"symbol": ["multiple_items_allowed"]}
+    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
 
 class YFinanceShareStatisticsData(ShareStatisticsData):
     """YFinance Share Statistics Data."""
 
     __alias_dict__ = {
         "outstanding_shares": "sharesOutstanding",
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/futures.csv` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/helpers.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/providers/yfinance/openbb_yfinance/utils/references.py` & `openbb_nightly-4.1.7.dev202405100010/providers/yfinance/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_nightly-4.1.7.dev202405090009/pyproject.toml` & `openbb_nightly-4.1.7.dev202405100010/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "openbb-nightly"
-version = "4.1.7.dev202405090009"
+version = "4.1.7.dev202405100010"
 description = "OpenBB"
 authors = [ "OpenBB Team <hello@openbb.co>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "openbb"
 
 [[tool.poetry.packages]]
@@ -197,19 +197,19 @@
 aiohttp = "^3.9.0"
 ruff = "^0.1.6"
 requests-cache = "^1.1.0"
 pytest-freezegun = "^0.4.2"
 urllib3 = ">1.26.16"
 defusedxml = "^0.8.0rc2"
 xmltodict = "^0.13.0"
+aiohttp-client-cache = "^0.10.0"
+aiosqlite = "^0.19.0"
 lxml = "^5.2.1"
 random-user-agent = "^1.0.1"
 yfinance = "^0.2.27"
-aiohttp-client-cache = "^0.10.0"
-aiosqlite = "^0.19.0"
 nasdaq-data-link = "^1.0.4"
 exchange-calendars = "^4.2.8"
 finvizfinance = "0.14.7"
 scipy = "^1.10.0"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.1"
 pandas-ta = "^0.3.14b"
```

### Comparing `openbb_nightly-4.1.7.dev202405090009/PKG-INFO` & `openbb_nightly-4.1.7.dev202405100010/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-nightly
-Version: 4.1.7.dev202405090009
+Version: 4.1.7.dev202405100010
 Summary: OpenBB
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

