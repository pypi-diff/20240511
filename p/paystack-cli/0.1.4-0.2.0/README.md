# Comparing `tmp/paystack_cli-0.1.4.tar.gz` & `tmp/paystack_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paystack_cli-0.1.4.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `paystack_cli-0.1.4.tar` & `paystack_cli-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-07-24 20:00:11.419052 paystack_cli-0.1.4/LICENSE
--rw-r--r--   0        0        0     1217 2023-12-01 19:57:05.141332 paystack_cli-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-07-19 21:04:35.944414 paystack_cli-0.1.4/paystack_cli/__init__.py
--rw-r--r--   0        0        0     1104 2023-07-27 09:42:56.394895 paystack_cli-0.1.4/paystack_cli/apple_pay.py
--rw-r--r--   0        0        0     3072 2023-07-24 17:35:10.884307 paystack_cli-0.1.4/paystack_cli/bulk_charges.py
--rw-r--r--   0        0        0     3835 2023-12-01 19:15:52.177857 paystack_cli-0.1.4/paystack_cli/charge.py
--rw-r--r--   0        0        0     3729 2023-07-24 17:35:10.924306 paystack_cli-0.1.4/paystack_cli/customers.py
--rw-r--r--   0        0        0     4782 2023-12-01 19:32:15.243034 paystack_cli-0.1.4/paystack_cli/dedicated_virtual_accounts.py
--rw-r--r--   0        0        0     3713 2023-07-24 17:40:00.337132 paystack_cli-0.1.4/paystack_cli/disputes.py
--rw-r--r--   0        0        0      710 2023-07-24 17:42:15.102544 paystack_cli-0.1.4/paystack_cli/integration.py
--rw-r--r--   0        0        0     7133 2023-12-01 19:11:38.573286 paystack_cli-0.1.4/paystack_cli/main.py
--rw-r--r--   0        0        0     1451 2023-12-01 19:22:28.891158 paystack_cli-0.1.4/paystack_cli/miscellaneous.py
--rw-r--r--   0        0        0     2788 2023-12-01 19:30:50.391009 paystack_cli-0.1.4/paystack_cli/payment_pages.py
--rw-r--r--   0        0        0     4479 2023-07-24 17:57:32.464325 paystack_cli-0.1.4/paystack_cli/payments_requests.py
--rw-r--r--   0        0        0     2093 2023-07-24 18:00:45.079200 paystack_cli-0.1.4/paystack_cli/plans.py
--rw-r--r--   0        0        0     1920 2023-07-24 18:04:03.576117 paystack_cli-0.1.4/paystack_cli/products.py
--rw-r--r--   0        0        0     1564 2023-07-24 18:06:12.699501 paystack_cli-0.1.4/paystack_cli/refunds.py
--rw-r--r--   0        0        0     1231 2023-07-24 18:09:03.792597 paystack_cli-0.1.4/paystack_cli/settlements.py
--rw-r--r--   0        0        0     3306 2023-07-24 18:12:46.875562 paystack_cli-0.1.4/paystack_cli/subaccounts.py
--rw-r--r--   0        0        0     2384 2023-07-24 18:16:37.889155 paystack_cli-0.1.4/paystack_cli/subscriptions.py
--rw-r--r--   0        0        0     2945 2023-07-24 18:28:41.008662 paystack_cli-0.1.4/paystack_cli/terminals.py
--rw-r--r--   0        0        0     5833 2023-12-01 19:30:50.401009 paystack_cli-0.1.4/paystack_cli/transactions.py
--rw-r--r--   0        0        0     2892 2023-07-24 18:36:11.984984 paystack_cli-0.1.4/paystack_cli/transactions_splits.py
--rw-r--r--   0        0        0     3150 2023-07-24 18:40:01.466531 paystack_cli-0.1.4/paystack_cli/transfer_recipients.py
--rw-r--r--   0        0        0     2447 2023-07-24 18:43:01.438487 paystack_cli-0.1.4/paystack_cli/transfers.py
--rw-r--r--   0        0        0     2044 2023-07-26 18:59:23.008137 paystack_cli-0.1.4/paystack_cli/transfers_control.py
--rw-r--r--   0        0        0     3437 2023-12-01 19:30:03.423203 paystack_cli-0.1.4/paystack_cli/utils.py
--rw-r--r--   0        0        0     1552 2023-07-24 18:51:27.954669 paystack_cli-0.1.4/paystack_cli/verification.py
--rw-r--r--   0        0        0      835 2023-12-01 19:20:30.517568 paystack_cli-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 paystack_cli-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/.python-version
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/Makefile
+-rw-r--r--   0        0        0   121432 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/paystack-cli.png
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/requirements.lock
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/__main__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/apple_pay.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/bulk_charges.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/charge.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/customers.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/dedicated_virtual_accounts.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/disputes.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/integration.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/miscellaneous.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/payment_pages.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/payments_requests.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/plans.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/products.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/refunds.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/settlements.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/subaccounts.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/subscriptions.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/terminals.py
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/transactions.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/transactions_splits.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/transfer_recipients.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/transfers.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/transfers_control.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/utils.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/src/paystack_cli/verification.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/README.md
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5595 2020-02-02 00:00:00.000000 paystack_cli-0.2.0/PKG-INFO
```

### Comparing `paystack_cli-0.1.4/LICENSE` & `paystack_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/apple_pay.py` & `paystack_cli-0.2.0/src/paystack_cli/apple_pay.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/bulk_charges.py` & `paystack_cli-0.2.0/src/paystack_cli/bulk_charges.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/charge.py` & `paystack_cli-0.2.0/src/paystack_cli/charge.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/customers.py` & `paystack_cli-0.2.0/src/paystack_cli/customers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/dedicated_virtual_accounts.py` & `paystack_cli-0.2.0/src/paystack_cli/dedicated_virtual_accounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/disputes.py` & `paystack_cli-0.2.0/src/paystack_cli/disputes.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/integration.py` & `paystack_cli-0.2.0/src/paystack_cli/integration.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/main.py` & `paystack_cli-0.2.0/src/paystack_cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typer import Typer
 from rich import print as rprint
+from typer import Typer
 
-from paystack_cli.charge import charge_app
-from paystack_cli.miscellaneous import miscellaneous_app
 from paystack_cli.apple_pay import app_pay_app
 from paystack_cli.bulk_charges import bulk_charge_app
+from paystack_cli.charge import charge_app
 from paystack_cli.customers import customer_app
 from paystack_cli.dedicated_virtual_accounts import dva_app
 from paystack_cli.disputes import dispute_app
 from paystack_cli.integration import integration_app
+from paystack_cli.miscellaneous import miscellaneous_app
 from paystack_cli.payment_pages import payment_page_app
 from paystack_cli.payments_requests import payment_request_app
 from paystack_cli.plans import plan_app
 from paystack_cli.products import product_app
 from paystack_cli.refunds import refund_app
 from paystack_cli.settlements import settlement_app
 from paystack_cli.subaccounts import subaccount_app
@@ -226,16 +226,8 @@
     reset_settings()
     rprint("auth key cleared! :boom:")
 
 
 @app.command()
 def version():
     """See CLI version"""
-    rprint("Paystack CLI Version 0.1.4")
-
-
-def run():
-    app()
-
-
-if __name__ == "__main__":
-    run()
+    rprint("Paystack CLI Version 0.2.0")
```

### Comparing `paystack_cli-0.1.4/paystack_cli/miscellaneous.py` & `paystack_cli-0.2.0/src/paystack_cli/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/payment_pages.py` & `paystack_cli-0.2.0/src/paystack_cli/payment_pages.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/payments_requests.py` & `paystack_cli-0.2.0/src/paystack_cli/payments_requests.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/plans.py` & `paystack_cli-0.2.0/src/paystack_cli/plans.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/products.py` & `paystack_cli-0.2.0/src/paystack_cli/products.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/refunds.py` & `paystack_cli-0.2.0/src/paystack_cli/refunds.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/settlements.py` & `paystack_cli-0.2.0/src/paystack_cli/settlements.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/subaccounts.py` & `paystack_cli-0.2.0/src/paystack_cli/subaccounts.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/subscriptions.py` & `paystack_cli-0.2.0/src/paystack_cli/subscriptions.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/terminals.py` & `paystack_cli-0.2.0/src/paystack_cli/terminals.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/transactions.py` & `paystack_cli-0.2.0/src/paystack_cli/transactions.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     return get_paystack_wrapper().transactions.get_transaction(id=id)
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def get_txns(
-    customer_id: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    status: Optional[TransactionStatus] = None,
-    page: Optional[int] = None,
-    amount: Optional[int] = None,
-    pagination: int = 50,
-    data_only: bool = False,
+        customer_id: Optional[str] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        status: Optional[TransactionStatus] = None,
+        page: Optional[int] = None,
+        amount: Optional[int] = None,
+        pagination: int = 50,
+        data_only: bool = False,
 ):
     """Fetch transactions carried out on your integration."""
     return get_paystack_wrapper().transactions.get_transactions(
         customer=customer_id,
         start_date=start_date,
         end_date=end_date,
         status=status,
@@ -54,26 +54,26 @@
     return get_paystack_wrapper().transactions.get_timeline(id_or_ref=id_or_ref)
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def charge(
-    amount: int,
-    email: str,
-    auth_code: str,
-    reference: Optional[str] = None,
-    currency: Optional[Currency] = None,
-    metadata: Optional[str] = None,
-    channels: Optional[list[Channel]] = None,
-    subaccount: Optional[str] = None,
-    transaction_charge: Optional[int] = None,
-    bearer: Optional[Bearer] = None,
-    queue: bool = False,
-    data_only: bool = False,
+        amount: int,
+        email: str,
+        auth_code: str,
+        reference: Optional[str] = None,
+        currency: Optional[Currency] = None,
+        metadata: Optional[str] = None,
+        channels: Optional[list[Channel]] = None,
+        subaccount: Optional[str] = None,
+        transaction_charge: Optional[int] = None,
+        bearer: Optional[Bearer] = None,
+        queue: bool = False,
+        data_only: bool = False,
 ):
     """All authorizations marked as reusable can be charged with this endpoint whenever you need to receive payments."""
     if metadata:
         metadata = parse_cli_string(
             raw_string=metadata, arg_or_option_name="metadata", expected_type=dict
         )
     return get_paystack_wrapper().transactions.charge(
@@ -91,26 +91,26 @@
     )
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def export(
-    page: Optional[int] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    customer_id: Optional[str] = None,
-    status: Optional[TransactionStatus] = None,
-    currency: Optional[Currency] = None,
-    amount: Optional[int] = None,
-    settled: Optional[bool] = None,
-    settlement_id: Optional[int] = None,
-    payment_page: Optional[int] = None,
-    pagination: int = 50,
-    data_only: bool = False,
+        page: Optional[int] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        customer_id: Optional[str] = None,
+        status: Optional[TransactionStatus] = None,
+        currency: Optional[Currency] = None,
+        amount: Optional[int] = None,
+        settled: Optional[bool] = None,
+        settlement_id: Optional[int] = None,
+        payment_page: Optional[int] = None,
+        pagination: int = 50,
+        data_only: bool = False,
 ):
     """Fetch transactions carried out on your integration."""
     return get_paystack_wrapper().transactions.export(
         page=page,
         start_date=start_date,
         end_date=end_date,
         customer=customer_id,
@@ -124,28 +124,28 @@
     )
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def init(
-    amount: int,
-    email: str,
-    currency: Optional[Currency] = None,
-    reference: Optional[str] = None,
-    callback_url: Optional[str] = None,
-    plan_id: Optional[str] = None,
-    invoice_limit: Optional[int] = None,
-    metadata: Optional[str] = None,
-    channels: Optional[list[Channel]] = None,
-    split_code: Optional[str] = None,
-    subaccount: Optional[str] = None,
-    transfer_charge: Optional[int] = None,
-    bearer: Optional[Bearer] = None,
-    data_only: bool = False,
+        amount: int,
+        email: str,
+        currency: Optional[Currency] = None,
+        reference: Optional[str] = None,
+        callback_url: Optional[str] = None,
+        plan_id: Optional[str] = None,
+        invoice_limit: Optional[int] = None,
+        metadata: Optional[str] = None,
+        channels: Optional[list[Channel]] = None,
+        split_code: Optional[str] = None,
+        subaccount: Optional[str] = None,
+        transfer_charge: Optional[int] = None,
+        bearer: Optional[Bearer] = None,
+        data_only: bool = False,
 ):
     """Initialize a transaction"""
     if metadata:
         metadata = parse_cli_string(
             raw_string=metadata, arg_or_option_name="metadata", expected_type=dict
         )
     return get_paystack_wrapper().transactions.initialize(
@@ -165,21 +165,21 @@
     )
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def partial_debit(
-    auth_code: str,
-    currency: Currency,
-    amount: int,
-    email: str,
-    reference: Optional[str] = None,
-    at_least: Optional[int] = None,
-    data_only: bool = False,
+        auth_code: str,
+        currency: Currency,
+        amount: int,
+        email: str,
+        reference: Optional[str] = None,
+        at_least: Optional[int] = None,
+        data_only: bool = False,
 ):
     """Retrieve part of a payment from a customer"""
     get_paystack_wrapper().transactions.partial_debit(
         auth_code=auth_code,
         currency=currency,
         amount=amount,
         email=email,
@@ -188,19 +188,19 @@
     )
 
 
 @transaction_app.command()
 @colorized_print
 @override_output
 def totals(
-    page: Optional[int] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    pagination: int = 50,
-    data_only: bool = False,
+        page: Optional[int] = None,
+        start_date: Optional[str] = None,
+        end_date: Optional[str] = None,
+        pagination: int = 50,
+        data_only: bool = False,
 ):
     """Total amount received on your account"""
     get_paystack_wrapper().transactions.totals(
         page=page, start_date=start_date, end_date=end_date, pagination=pagination
     )
```

### Comparing `paystack_cli-0.1.4/paystack_cli/transactions_splits.py` & `paystack_cli-0.2.0/src/paystack_cli/transactions_splits.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/transfer_recipients.py` & `paystack_cli-0.2.0/src/paystack_cli/transfer_recipients.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/transfers.py` & `paystack_cli-0.2.0/src/paystack_cli/transfers.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/transfers_control.py` & `paystack_cli-0.2.0/src/paystack_cli/transfers_control.py`

 * *Files identical despite different names*

### Comparing `paystack_cli-0.1.4/paystack_cli/utils.py` & `paystack_cli-0.2.0/src/paystack_cli/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import functools
 import json
 import os.path
+from json import JSONDecodeError
 from pathlib import Path
 from typing import Optional, Type
 
+import httpx
 import typer
 from pypaystack2 import Paystack
 from rich import print as rprint
 from typer import get_app_dir
 
 APP_CONFIG_DIR_NAME = ".paystack-cli"
 
@@ -62,15 +64,15 @@
             "[bold red]Error![/bold red] your auth key has not been configured. please run `paystack config <auth_key>`"
         )
         raise typer.Abort()
     return Paystack(auth_key=auth_key)
 
 
 def parse_cli_string(
-    raw_string: str, arg_or_option_name: str, expected_type: Type, many: bool = False
+        raw_string: str, arg_or_option_name: str, expected_type: Type, many: bool = False
 ):
     """parses the json encoded string gotten form the cli input to the expected type.
 
     Args:
         raw_string: the json decodable value passed in by the user to the cli to be parsed into the expected type.
         arg_or_option_name: the name of the cli argument or option.
         expected_type: the expected type
@@ -81,33 +83,41 @@
         parsed_data = json.loads(raw_string)
         if isinstance(parsed_data, expected_type):
             return parsed_data
         if isinstance(parsed_data, dict) and not many:
             return expected_type(**parsed_data)
         if isinstance(parsed_data, list) and many:
             return [expected_type(**item) for item in parsed_data]
-    except json.decoder.JSONDecodeError:
+    except (json.decoder.JSONDecodeError, TypeError):
         rprint(
             f"[bold red]Error![/bold red] unable to parse value in `{arg_or_option_name}` option or argument, expects a json decodable string"
             f" that can be parsed into a {'`list` of ' if many else ''}`{expected_type.__name__}`"
         )
-        raise typer.Abort()
+        raise typer.Exit(code=1)
 
 
 def colorized_print(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         response = func(*args, **kwargs)
         rprint(response)
 
     return wrapper
 
 
 def override_output(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
-        response = func(*args, **kwargs)
+        try:
+            response = func(*args, **kwargs)
+        except httpx.RequestError as error:
+            rprint(f"an error occurred while making a request to paystack: error: {error}")
+            raise typer.Exit(code=1)
         if kwargs["data_only"]:
-            return response.data
+            try:
+                return json.dumps(response.data)
+            except (JSONDecodeError, TypeError):
+                rprint(f"unable to decode data as json.\ngot: data: {response.data}\nmessage: {response.message}")
+                raise typer.Exit(code=1)
         return response
 
     return wrapper
```

### Comparing `paystack_cli-0.1.4/paystack_cli/verification.py` & `paystack_cli-0.2.0/src/paystack_cli/verification.py`

 * *Files identical despite different names*

