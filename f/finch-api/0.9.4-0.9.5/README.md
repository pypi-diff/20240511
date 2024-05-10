# Comparing `tmp/finch_api-0.9.4.tar.gz` & `tmp/finch_api-0.9.5.tar.gz`

## Comparing `finch_api-0.9.4.tar` & `finch_api-0.9.5.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/__init__.py
--rw-r--r--   0        0        0    57627 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_base_client.py
--rw-r--r--   0        0        0    24950 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_client.py
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_compat.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_constants.py
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_exceptions.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_files.py
--rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_qs.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_resource.py
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_response.py
--rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_streaming.py
--rw-r--r--   0        0        0    10056 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_types.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_version.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/py.typed
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/__init__.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_logs.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_streams.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_transform.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_typing.py
--rw-r--r--   0        0        0    11024 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/_utils/_utils.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/__init__.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/account.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/providers.py
--rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/request_forwarding.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/webhooks.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/company.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/directory.py
--rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/employments.py
--rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/hris.py
--rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/individuals.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/pay_statements.py
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/payments.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/benefits/__init__.py
--rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/benefits/benefits.py
--rw-r--r--   0        0        0    16164 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/hris/benefits/individuals.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/jobs/__init__.py
--rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/jobs/automated.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/jobs/jobs.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/resources/jobs/manual.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/__init__.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/disconnect_response.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/income.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/introspection.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/location.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/money.py
--rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/provider.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/request_forwarding_forward_params.py
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/request_forwarding_forward_response.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_contribution.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_create_params.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_features_and_operations.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_frequency.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_type.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefit_update_params.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits_support.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benfit_contribution.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/company.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/company_benefit.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/create_company_benefits_response.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/directory_list_individuals_params.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/directory_list_params.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/employment_data.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/employment_data_response.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/employment_retrieve_many_params.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/individual.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/individual_in_directory.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/individual_response.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/individual_retrieve_many_params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/pay_statement.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/pay_statement_response.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/pay_statement_response_body.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/pay_statement_retrieve_many_params.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/payment.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/payment_list_params.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/support_per_benefit_type.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/supported_benefit.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/update_company_benefit_response.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/__init__.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/enrolled_individual.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/individual_benefit.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/individual_enroll_many_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/individual_unenroll_many_params.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/hris/benefits/unenrolled_individual.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/__init__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/automated_async_job.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/automated_create_params.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/automated_create_response.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/automated_list_params.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/jobs/manual_async_job.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/shared/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/shared/operation_support.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/shared/operation_support_matrix.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 finch_api-0.9.4/src/finch/types/shared/paging.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 finch_api-0.9.4/.gitignore
--rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 finch_api-0.9.4/LICENSE
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 finch_api-0.9.4/README.md
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 finch_api-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 finch_api-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/__init__.py
+-rw-r--r--   0        0        0    57627 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_base_client.py
+-rw-r--r--   0        0        0    24950 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_client.py
+-rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_compat.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_constants.py
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_exceptions.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_files.py
+-rw-r--r--   0        0        0    16467 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_qs.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_resource.py
+-rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_response.py
+-rw-r--r--   0        0        0     7096 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_streaming.py
+-rw-r--r--   0        0        0    10068 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_types.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_version.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/py.typed
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/__init__.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_logs.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_streams.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_transform.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_typing.py
+-rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/_utils/_utils.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/__init__.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/account.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/providers.py
+-rw-r--r--   0        0        0     7338 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/request_forwarding.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/webhooks.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/company.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/directory.py
+-rw-r--r--   0        0        0     5168 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/employments.py
+-rw-r--r--   0        0        0     3920 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/hris.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/individuals.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/pay_statements.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/payments.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/benefits/__init__.py
+-rw-r--r--   0        0        0    16194 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/benefits/benefits.py
+-rw-r--r--   0        0        0    16164 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/hris/benefits/individuals.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/jobs/__init__.py
+-rw-r--r--   0        0        0    12197 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/jobs/automated.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/jobs/jobs.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/resources/jobs/manual.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/disconnect_response.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/income.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/introspection.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/location.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/money.py
+-rw-r--r--   0        0        0    12502 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/provider.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/request_forwarding_forward_params.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/request_forwarding_forward_response.py
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_contribution.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_create_params.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_features_and_operations.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_frequency.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_type.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefit_update_params.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits_support.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benfit_contribution.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/company.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/company_benefit.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/create_company_benefits_response.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/directory_list_individuals_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/directory_list_params.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/employment_data.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/employment_data_response.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/employment_retrieve_many_params.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/individual.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/individual_in_directory.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/individual_response.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/individual_retrieve_many_params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/pay_statement.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/pay_statement_response.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/pay_statement_response_body.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/pay_statement_retrieve_many_params.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/payment.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/payment_list_params.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/support_per_benefit_type.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/supported_benefit.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/update_company_benefit_response.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/__init__.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/enrolled_individual.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/individual_benefit.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/individual_enroll_many_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/individual_enrolled_ids_response.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/individual_retrieve_many_benefits_params.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/individual_unenroll_many_params.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/hris/benefits/unenrolled_individual.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/__init__.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/automated_async_job.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/automated_create_params.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/automated_create_response.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/automated_list_params.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/jobs/manual_async_job.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/shared/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/shared/operation_support.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/shared/operation_support_matrix.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 finch_api-0.9.5/src/finch/types/shared/paging.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 finch_api-0.9.5/.gitignore
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 finch_api-0.9.5/LICENSE
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 finch_api-0.9.5/README.md
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 finch_api-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    12206 2020-02-02 00:00:00.000000 finch_api-0.9.5/PKG-INFO
```

### Comparing `finch_api-0.9.4/src/finch/__init__.py` & `finch_api-0.9.5/src/finch/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_base_client.py` & `finch_api-0.9.5/src/finch/_base_client.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_client.py` & `finch_api-0.9.5/src/finch/_client.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_compat.py` & `finch_api-0.9.5/src/finch/_compat.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_exceptions.py` & `finch_api-0.9.5/src/finch/_exceptions.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_files.py` & `finch_api-0.9.5/src/finch/_files.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_models.py` & `finch_api-0.9.5/src/finch/_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
 
     class RootModel(GenericModel, Generic[_T]):
         """Used as a placeholder to easily convert runtime types to a Pydantic format
         to provide validation.
 
         For example:
         ```py
-        validated = RootModel[int](__root__='5').__root__
+        validated = RootModel[int](__root__="5").__root__
         # validated: 5
         ```
         """
 
         __root__: _T
 
     def _validate_non_model_type(*, type_: type[_T], value: object) -> _T:
```

### Comparing `finch_api-0.9.4/src/finch/_qs.py` & `finch_api-0.9.5/src/finch/_qs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_resource.py` & `finch_api-0.9.5/src/finch/_resource.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_response.py` & `finch_api-0.9.5/src/finch/_response.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_streaming.py` & `finch_api-0.9.5/src/finch/_streaming.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_types.py` & `finch_api-0.9.5/src/finch/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,19 +274,21 @@
     """
     A sentinel singleton class used to distinguish omitted keyword arguments
     from those passed in with the value None (which may have different behavior).
 
     For example:
 
     ```py
-    def get(timeout: Union[int, NotGiven, None] = NotGiven()) -> Response: ...
+    def get(timeout: Union[int, NotGiven, None] = NotGiven()) -> Response:
+        ...
 
-    get(timeout=1) # 1s timeout
-    get(timeout=None) # No timeout
-    get() # Default timeout behavior, which may not be statically known at the method definition.
+
+    get(timeout=1)  # 1s timeout
+    get(timeout=None)  # No timeout
+    get()  # Default timeout behavior, which may not be statically known at the method definition.
     ```
     """
 
     def __bool__(self) -> Literal[False]:
         return False
 
     @override
@@ -300,22 +302,22 @@
 
 class Omit:
     """In certain situations you need to be able to represent a case where a default value has
     to be explicitly removed and `None` is not an appropriate substitute, for example:
 
     ```py
     # as the default `Content-Type` header is `application/json` that will be sent
-    client.post('/upload/files', files={'file': b'my raw file content'})
+    client.post("/upload/files", files={"file": b"my raw file content"})
 
     # you can't explicitly override the header as it has to be dynamically generated
     # to look something like: 'multipart/form-data; boundary=0d8382fcf5f8c3be01ca2e11002d2983'
-    client.post(..., headers={'Content-Type': 'multipart/form-data'})
+    client.post(..., headers={"Content-Type": "multipart/form-data"})
 
     # instead you can remove the default `application/json` header by passing Omit
-    client.post(..., headers={'Content-Type': Omit()})
+    client.post(..., headers={"Content-Type": Omit()})
     ```
     """
 
     def __bool__(self) -> Literal[False]:
         return False
```

### Comparing `finch_api-0.9.4/src/finch/pagination.py` & `finch_api-0.9.5/src/finch/pagination.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_utils/__init__.py` & `finch_api-0.9.5/src/finch/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_utils/_logs.py` & `finch_api-0.9.5/src/finch/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_utils/_proxy.py` & `finch_api-0.9.5/src/finch/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_utils/_transform.py` & `finch_api-0.9.5/src/finch/_utils/_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,18 @@
     data: _T,
     expected_type: object,
 ) -> _T:
     """Transform dictionaries based off of type information from the given type, for example:
 
     ```py
     class Params(TypedDict, total=False):
-        card_id: Required[Annotated[str, PropertyInfo(alias='cardID')]]
+        card_id: Required[Annotated[str, PropertyInfo(alias="cardID")]]
 
-    transformed = transform({'card_id': '<my card ID>'}, Params)
+
+    transformed = transform({"card_id": "<my card ID>"}, Params)
     # {'cardID': '<my card ID>'}
     ```
 
     Any keys / data that does not have type information given will be included as is.
 
     It should be noted that the transformations that this function does are not represented in the type system.
     """
```

### Comparing `finch_api-0.9.4/src/finch/_utils/_typing.py` & `finch_api-0.9.5/src/finch/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/_utils/_utils.py` & `finch_api-0.9.5/src/finch/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,21 +207,23 @@
 
     Example usage:
     ```py
     @overload
     def foo(*, a: str) -> str:
         ...
 
+
     @overload
     def foo(*, b: bool) -> str:
         ...
 
+
     # This enforces the same constraints that a static type checker would
     # i.e. that either a or b must be passed to the function
-    @required_args(['a'], ['b'])
+    @required_args(["a"], ["b"])
     def foo(*, a: str | None = None, b: bool | None = None) -> str:
         ...
     ```
     """
 
     def inner(func: CallableT) -> CallableT:
         params = inspect.signature(func).parameters
```

### Comparing `finch_api-0.9.4/src/finch/resources/__init__.py` & `finch_api-0.9.5/src/finch/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/account.py` & `finch_api-0.9.5/src/finch/resources/account.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/providers.py` & `finch_api-0.9.5/src/finch/resources/providers.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/request_forwarding.py` & `finch_api-0.9.5/src/finch/resources/request_forwarding.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/webhooks.py` & `finch_api-0.9.5/src/finch/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/__init__.py` & `finch_api-0.9.5/src/finch/resources/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/company.py` & `finch_api-0.9.5/src/finch/resources/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/directory.py` & `finch_api-0.9.5/src/finch/resources/hris/directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/employments.py` & `finch_api-0.9.5/src/finch/resources/hris/employments.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/hris.py` & `finch_api-0.9.5/src/finch/resources/hris/hris.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/individuals.py` & `finch_api-0.9.5/src/finch/resources/hris/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/pay_statements.py` & `finch_api-0.9.5/src/finch/resources/hris/pay_statements.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/payments.py` & `finch_api-0.9.5/src/finch/resources/hris/payments.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/benefits/__init__.py` & `finch_api-0.9.5/src/finch/resources/hris/benefits/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/benefits/benefits.py` & `finch_api-0.9.5/src/finch/resources/hris/benefits/benefits.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/hris/benefits/individuals.py` & `finch_api-0.9.5/src/finch/resources/hris/benefits/individuals.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/jobs/__init__.py` & `finch_api-0.9.5/src/finch/resources/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/jobs/automated.py` & `finch_api-0.9.5/src/finch/resources/jobs/automated.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/jobs/jobs.py` & `finch_api-0.9.5/src/finch/resources/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/resources/jobs/manual.py` & `finch_api-0.9.5/src/finch/resources/jobs/manual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/__init__.py` & `finch_api-0.9.5/src/finch/types/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/income.py` & `finch_api-0.9.5/src/finch/types/income.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/introspection.py` & `finch_api-0.9.5/src/finch/types/introspection.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/location.py` & `finch_api-0.9.5/src/finch/types/location.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/provider.py` & `finch_api-0.9.5/src/finch/types/provider.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/request_forwarding_forward_params.py` & `finch_api-0.9.5/src/finch/types/request_forwarding_forward_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/request_forwarding_forward_response.py` & `finch_api-0.9.5/src/finch/types/request_forwarding_forward_response.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/__init__.py` & `finch_api-0.9.5/src/finch/types/hris/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefit_features_and_operations.py` & `finch_api-0.9.5/src/finch/types/hris/benefit_features_and_operations.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefit_type.py` & `finch_api-0.9.5/src/finch/types/hris/benefit_type.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits_support.py` & `finch_api-0.9.5/src/finch/types/hris/benefits_support.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/company.py` & `finch_api-0.9.5/src/finch/types/hris/company.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/company_benefit.py` & `finch_api-0.9.5/src/finch/types/hris/company_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/employment_data.py` & `finch_api-0.9.5/src/finch/types/hris/employment_data.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/employment_retrieve_many_params.py` & `finch_api-0.9.5/src/finch/types/hris/employment_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/individual.py` & `finch_api-0.9.5/src/finch/types/hris/individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/individual_in_directory.py` & `finch_api-0.9.5/src/finch/types/hris/individual_in_directory.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/pay_statement.py` & `finch_api-0.9.5/src/finch/types/hris/pay_statement.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/pay_statement_retrieve_many_params.py` & `finch_api-0.9.5/src/finch/types/hris/pay_statement_retrieve_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/payment.py` & `finch_api-0.9.5/src/finch/types/hris/payment.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/payment_list_params.py` & `finch_api-0.9.5/src/finch/types/hris/payment_list_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/supported_benefit.py` & `finch_api-0.9.5/src/finch/types/hris/supported_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits/__init__.py` & `finch_api-0.9.5/src/finch/types/hris/benefits/__init__.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits/enrolled_individual.py` & `finch_api-0.9.5/src/finch/types/hris/benefits/enrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits/individual_benefit.py` & `finch_api-0.9.5/src/finch/types/hris/benefits/individual_benefit.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits/individual_enroll_many_params.py` & `finch_api-0.9.5/src/finch/types/hris/benefits/individual_enroll_many_params.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/hris/benefits/unenrolled_individual.py` & `finch_api-0.9.5/src/finch/types/hris/benefits/unenrolled_individual.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/jobs/automated_async_job.py` & `finch_api-0.9.5/src/finch/types/jobs/automated_async_job.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/jobs/automated_create_response.py` & `finch_api-0.9.5/src/finch/types/jobs/automated_create_response.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/src/finch/types/shared/operation_support_matrix.py` & `finch_api-0.9.5/src/finch/types/shared/operation_support_matrix.py`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/LICENSE` & `finch_api-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/README.md` & `finch_api-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `finch_api-0.9.4/pyproject.toml` & `finch_api-0.9.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "finch-api"
-version = "0.9.4"
+version = "0.9.5"
 description = "The official Python library for the Finch API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Finch", email = "founders@tryfinch.com" },
 ]
 dependencies = [
@@ -45,39 +45,40 @@
 
 [tool.rye]
 managed = true
 # version pins are in requirements-dev.lock
 dev-dependencies = [
     "pyright",
     "mypy",
-    "black",
     "respx",
     "pytest",
     "pytest-asyncio",
     "ruff",
     "isort",
     "time-machine",
     "nox",
     "dirty-equals>=0.6.0",
+    "importlib-metadata>=6.7.0",
 
 ]
 
 [tool.rye.scripts]
 format = { chain = [
-  "format:black",
-  "format:docs",
   "format:ruff",
+  "format:docs",
+  "fix:ruff",
   "format:isort",
 ]}
 "format:black" = "black ."
-"format:docs" = "python bin/blacken-docs.py README.md api.md"
-"format:ruff" = "ruff --fix ."
+"format:docs" = "python bin/ruffen-docs.py README.md api.md"
+"format:ruff" = "ruff format"
 "format:isort" = "isort ."
 
 "check:ruff" = "ruff ."
+"fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
 "typecheck:verify-types" = "pyright --verifytypes finch --ignoreexternal"
@@ -155,12 +156,14 @@
 unfixable = [
   # disable auto fix for print statements
   "T201",
   "T203",
 ]
 ignore-init-module-imports = true
 
+[tool.ruff.format]
+docstring-code-format = true
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `finch_api-0.9.4/PKG-INFO` & `finch_api-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finch-api
-Version: 0.9.4
+Version: 0.9.5
 Summary: The official Python library for the Finch API
 Project-URL: Homepage, https://github.com/Finch-API/finch-api-python
 Project-URL: Repository, https://github.com/Finch-API/finch-api-python
 Author-email: Finch <founders@tryfinch.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

