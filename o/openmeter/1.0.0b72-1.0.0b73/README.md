# Comparing `tmp/openmeter-1.0.0b72.tar.gz` & `tmp/openmeter-1.0.0b73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmeter-1.0.0b72.tar", max compression
+gzip compressed data, was "openmeter-1.0.0b73.tar", max compression
```

## Comparing `openmeter-1.0.0b72.tar` & `openmeter-1.0.0b73.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1260 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/README.md
--rw-r--r--   0        0        0      837 2024-05-07 23:19:59.283640 openmeter-1.0.0b72/pyproject.toml
--rw-r--r--   0        0        0      702 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/__init__.py
--rw-r--r--   0        0        0     3982 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_client.py
--rw-r--r--   0        0        0     1807 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_operations/__init__.py
--rw-r--r--   0        0        0   178032 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_operations/_operations.py
--rw-r--r--   0        0        0     4874 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_patch.py
--rw-r--r--   0        0        0    78873 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_serialization.py
--rw-r--r--   0        0        0      851 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/_vendor.py
--rw-r--r--   0        0        0      702 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/__init__.py
--rw-r--r--   0        0        0     4100 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_client.py
--rw-r--r--   0        0        0     1817 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_configuration.py
--rw-r--r--   0        0        0      682 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_operations/__init__.py
--rw-r--r--   0        0        0   156302 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_operations/_operations.py
--rw-r--r--   0        0        0      674 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_operations/_patch.py
--rw-r--r--   0        0        0      674 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_patch.py
--rw-r--r--   0        0        0      862 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/aio/_vendor.py
--rw-r--r--   0        0        0       26 2024-05-07 23:10:46.000000 openmeter-1.0.0b72/src/openmeter/py.typed
--rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b72/PKG-INFO
+-rw-r--r--   0        0        0     1260 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/README.md
+-rw-r--r--   0        0        0      837 2024-05-11 09:10:09.645854 openmeter-1.0.0b73/pyproject.toml
+-rw-r--r--   0        0        0      702 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/__init__.py
+-rw-r--r--   0        0        0     3982 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_client.py
+-rw-r--r--   0        0        0     1807 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/__init__.py
+-rw-r--r--   0        0        0   177834 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/_operations.py
+-rw-r--r--   0        0        0     4874 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_patch.py
+-rw-r--r--   0        0        0    78873 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_serialization.py
+-rw-r--r--   0        0        0      851 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/_vendor.py
+-rw-r--r--   0        0        0      702 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/__init__.py
+-rw-r--r--   0        0        0     4100 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_client.py
+-rw-r--r--   0        0        0     1817 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_configuration.py
+-rw-r--r--   0        0        0      682 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/__init__.py
+-rw-r--r--   0        0        0   156104 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/_operations.py
+-rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_operations/_patch.py
+-rw-r--r--   0        0        0      674 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_patch.py
+-rw-r--r--   0        0        0      862 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/aio/_vendor.py
+-rw-r--r--   0        0        0       26 2024-05-10 09:48:14.000000 openmeter-1.0.0b73/src/openmeter/py.typed
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 openmeter-1.0.0b73/PKG-INFO
```

### Comparing `openmeter-1.0.0b72/README.md` & `openmeter-1.0.0b73/README.md`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/pyproject.toml` & `openmeter-1.0.0b73/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openmeter"
-version = "v1.0.0-beta.72"
+version = "v1.0.0-beta.73"
 description = "Client for OpenMeter: Real-Time and Scalable Usage Metering"
 authors = ["Andras Toth <4157749+tothandras@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/openmeter/openmeter"
 homepage = "https://openmeter.io"
 keywords = [
```

### Comparing `openmeter-1.0.0b72/src/openmeter/__init__.py` & `openmeter-1.0.0b73/src/openmeter/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_client.py` & `openmeter-1.0.0b73/src/openmeter/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_configuration.py` & `openmeter-1.0.0b73/src/openmeter/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_operations/__init__.py` & `openmeter-1.0.0b73/src/openmeter/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_operations/_operations.py` & `openmeter-1.0.0b73/src/openmeter/_operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,15 +491,15 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_get_credit_balance_request(
+def build_get_ledger_balance_request(
     ledger_id: str, *, time: Optional[datetime.datetime] = None, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
@@ -517,15 +517,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_get_credit_history_request(
+def build_get_ledger_history_request(
     ledger_id: str,
     *,
     from_parameter: datetime.datetime,
     limit: int = 1000,
     to: Optional[datetime.datetime] = None,
     **kwargs: Any
 ) -> HttpRequest:
@@ -551,15 +551,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_reset_credit_request(ledger_id: str, **kwargs: Any) -> HttpRequest:
+def build_reset_ledger_request(ledger_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
     # Construct URL
     _url = "/api/v1/ledgers/{ledgerID}/reset"
@@ -573,15 +573,15 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_list_credit_grants_request(
+def build_list_ledger_grants_request(
     *, ledger_id: Optional[str] = None, limit: int = 1000, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
@@ -596,15 +596,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_list_credit_grants_by_ledger_request(  # pylint: disable=name-too-long
+def build_list_ledger_grants_by_ledger_request(  # pylint: disable=name-too-long
     ledger_id: str, *, limit: int = 1000, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
@@ -622,15 +622,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-def build_create_credit_grant_request(ledger_id: str, **kwargs: Any) -> HttpRequest:
+def build_create_ledger_grant_request(ledger_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
     # Construct URL
     _url = "/api/v1/ledgers/{ledgerID}/grants"
@@ -644,43 +644,43 @@
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
-def build_get_credit_grant_request(ledger_id: str, credit_grant_id: str, **kwargs: Any) -> HttpRequest:
+def build_get_ledger_grant_request(ledger_id: str, ledger_grant_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/json, application/problem+json")
 
     # Construct URL
-    _url = "/api/v1/ledgers/{ledgerID}/grants/{creditGrantID}"
+    _url = "/api/v1/ledgers/{ledgerID}/grants/{ledgerGrantID}"
     path_format_arguments = {
         "ledgerID": _SERIALIZER.url("ledger_id", ledger_id, "str"),
-        "creditGrantID": _SERIALIZER.url("credit_grant_id", credit_grant_id, "str"),
+        "ledgerGrantID": _SERIALIZER.url("ledger_grant_id", ledger_grant_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
-def build_void_credit_grant_request(credit_grant_id: str, ledger_id: str, **kwargs: Any) -> HttpRequest:
+def build_void_ledger_grant_request(ledger_grant_id: str, ledger_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     accept = _headers.pop("Accept", "application/problem+json")
 
     # Construct URL
-    _url = "/api/v1/ledgers/{ledgerID}/grants/{creditGrantID}"
+    _url = "/api/v1/ledgers/{ledgerID}/grants/{ledgerGrantID}"
     path_format_arguments = {
-        "creditGrantID": _SERIALIZER.url("credit_grant_id", credit_grant_id, "str"),
+        "ledgerGrantID": _SERIALIZER.url("ledger_grant_id", ledger_grant_id, "str"),
         "ledgerID": _SERIALIZER.url("ledger_id", ledger_id, "str"),
     }
 
     _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
@@ -2903,15 +2903,15 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "id": "str",  # Readonly unique ULID identifier of the ledger.
                           Required.
                         "subject": "str",  # The metering subject this ledger used to track
-                          credits for. Required.
+                          grants for. Required.
                         "metadata": {
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         }
                     }
                 ]
         """
         error_map = {
@@ -2976,25 +2976,25 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
 
@@ -3015,15 +3015,15 @@
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
 
@@ -3040,25 +3040,25 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
         error_map = {
@@ -3113,21 +3113,21 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def get_credit_balance(self, ledger_id: str, *, time: Optional[datetime.datetime] = None, **kwargs: Any) -> JSON:
+    def get_ledger_balance(self, ledger_id: str, *, time: Optional[datetime.datetime] = None, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
         """Get the balance of a specific subject.
 
         Get the balance of a specific subject.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword time: Point of time to query balances: date-time in RFC 3339 format. Defaults to now.
          Default value is None.
         :paramtype time: ~datetime.datetime
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -3167,19 +3167,18 @@
                                   :code:`<string>`.
                             },
                             "priority": 1,  # Optional. Default value is 1. The priority
                               of the grant. Grants with higher priority are applied first. Priority is
                               a positive decimal numbers. With lower numbers indicating higher
                               importance. For example, a priority of 1 is more urgent than a priority
                               of 2. When there are several grants available for the same subject, the
-                              system selects the grant with the highest priority. In cases where credit
-                              grants share the same priority level, the grant closest to its expiration
-                              will be used first. In the case of two credits have identical priorities
-                              and expiration dates, the system will use the grant that was created
-                              first.
+                              system selects the grant with the highest priority. In cases where grants
+                              share the same priority level, the grant closest to its expiration will
+                              be used first. In the case of two grants have identical priorities and
+                              expiration dates, the system will use the grant that was created first.
                             "rollover": {
                                 "type": "str",  # The rollover type to use:   *
                                   ``REMAINING_AMOUNT`` - Rollover remaining amount. *
                                   ``ORIGINAL_AMOUNT`` - Rollover re-applies the full grant amount.
                                   Required. Known values are: "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                                 "maxAmount": 0.0  # Optional. Maximum amount to
                                   rollover.
@@ -3214,15 +3213,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_balance_request(
+        _request = build_get_ledger_balance_request(
             ledger_id=ledger_id,
             time=time,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -3246,28 +3245,28 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def get_credit_history(
+    def get_ledger_history(
         self,
         ledger_id: str,
         *,
         from_parameter: datetime.datetime,
         limit: int = 1000,
         to: Optional[datetime.datetime] = None,
         **kwargs: Any
     ) -> List[JSON]:
-        """Get credit ledger.
+        """Get the history of a ledger.
 
-        Get credit ledger for a specific subject.
+        Get the history of a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword from_parameter: Start of time range to query ledger: date-time in RFC 3339 format.
          Required.
         :paramtype from_parameter: ~datetime.datetime
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
         :keyword to: End of time range to query ledger: date-time in RFC 3339 format. Defaults to now.
@@ -3309,15 +3308,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_history_request(
+        _request = build_get_ledger_history_request(
             ledger_id=ledger_id,
             from_parameter=from_parameter,
             limit=limit,
             to=to,
             headers=_headers,
             params=_params,
         )
@@ -3343,23 +3342,23 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def reset_credit(
+    def reset_ledger(
         self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
-        """Reset credit balance.
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Required.
         :type body: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
@@ -3367,37 +3366,37 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
 
     @overload
-    def reset_credit(
+    def reset_ledger(
         self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
-        """Reset credit balance.
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Required.
         :type body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
@@ -3405,48 +3404,48 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
 
     @distributed_trace
-    def reset_credit(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        """Reset credit balance.
+    def reset_ledger(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Is either a JSON type or a IO[bytes] type. Required.
         :type body: JSON or IO[bytes]
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
         error_map = {
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -3466,15 +3465,15 @@
         _json = None
         _content = None
         if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
-        _request = build_reset_credit_request(
+        _request = build_reset_ledger_request(
             ledger_id=ledger_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -3500,19 +3499,19 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def list_credit_grants(self, *, ledger_id: Optional[str] = None, limit: int = 1000, **kwargs: Any) -> List[JSON]:
+    def list_ledger_grants(self, *, ledger_id: Optional[str] = None, limit: int = 1000, **kwargs: Any) -> List[JSON]:
         # pylint: disable=line-too-long
-        """List credit grants for multiple ledgers.
+        """List grants for multiple ledgers.
 
-        List credit grants for multiple ledgers.
+        List grants for multiple ledgers.
 
         :keyword ledger_id: Filtering and group by multiple subjects.
 
          Usage: ``?ledgerID=01HX6VK5C498B3ABY9PR1069PP``. Default value is None.
         :paramtype ledger_id: str
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
@@ -3550,18 +3549,18 @@
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         },
                         "priority": 1,  # Optional. Default value is 1. The priority of the
                           grant. Grants with higher priority are applied first. Priority is a positive
                           decimal numbers. With lower numbers indicating higher importance. For
                           example, a priority of 1 is more urgent than a priority of 2. When there are
                           several grants available for the same subject, the system selects the grant
-                          with the highest priority. In cases where credit grants share the same
-                          priority level, the grant closest to its expiration will be used first. In
-                          the case of two credits have identical priorities and expiration dates, the
-                          system will use the grant that was created first.
+                          with the highest priority. In cases where grants share the same priority
+                          level, the grant closest to its expiration will be used first. In the case of
+                          two grants have identical priorities and expiration dates, the system will
+                          use the grant that was created first.
                         "rollover": {
                             "type": "str",  # The rollover type to use:   *
                               ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
                               Rollover re-applies the full grant amount. Required. Known values are:
                               "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                             "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                         }
@@ -3578,15 +3577,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_list_credit_grants_request(
+        _request = build_list_ledger_grants_request(
             ledger_id=ledger_id,
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -3610,21 +3609,21 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @distributed_trace
-    def list_credit_grants_by_ledger(self, ledger_id: str, *, limit: int = 1000, **kwargs: Any) -> List[JSON]:
+    def list_ledger_grants_by_ledger(self, ledger_id: str, *, limit: int = 1000, **kwargs: Any) -> List[JSON]:
         # pylint: disable=line-too-long
-        """List credit grants.
+        """List ledger grants.
 
-        List credit grants for a specific ledger.
+        List ledger grants for a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
         :return: list of JSON object
         :rtype: list[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -3658,18 +3657,18 @@
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         },
                         "priority": 1,  # Optional. Default value is 1. The priority of the
                           grant. Grants with higher priority are applied first. Priority is a positive
                           decimal numbers. With lower numbers indicating higher importance. For
                           example, a priority of 1 is more urgent than a priority of 2. When there are
                           several grants available for the same subject, the system selects the grant
-                          with the highest priority. In cases where credit grants share the same
-                          priority level, the grant closest to its expiration will be used first. In
-                          the case of two credits have identical priorities and expiration dates, the
-                          system will use the grant that was created first.
+                          with the highest priority. In cases where grants share the same priority
+                          level, the grant closest to its expiration will be used first. In the case of
+                          two grants have identical priorities and expiration dates, the system will
+                          use the grant that was created first.
                         "rollover": {
                             "type": "str",  # The rollover type to use:   *
                               ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
                               Rollover re-applies the full grant amount. Required. Known values are:
                               "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                             "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                         }
@@ -3686,15 +3685,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_list_credit_grants_by_ledger_request(
+        _request = build_list_ledger_grants_by_ledger_request(
             ledger_id=ledger_id,
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -3718,25 +3717,25 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    def create_credit_grant(
+    def create_ledger_grant(
         self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Required.
+        :param body: The grant to create. Required.
         :type body: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -3763,16 +3762,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3802,40 +3801,40 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
                         "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                     }
                 }
         """
 
     @overload
-    def create_credit_grant(
+    def create_ledger_grant(
         self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Required.
+        :param body: The grant to create. Required.
         :type body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -3865,38 +3864,38 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
                         "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                     }
                 }
         """
 
     @distributed_trace
-    def create_credit_grant(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+    def create_ledger_grant(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Is either a JSON type or a IO[bytes] type. Required.
+        :param body: The grant to create. Is either a JSON type or a IO[bytes] type. Required.
         :type body: JSON or IO[bytes]
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
@@ -3920,16 +3919,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3959,16 +3958,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3995,15 +3994,15 @@
         _json = None
         _content = None
         if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
-        _request = build_create_credit_grant_request(
+        _request = build_create_ledger_grant_request(
             ledger_id=ledger_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -4029,24 +4028,24 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def get_credit_grant(self, ledger_id: str, credit_grant_id: str, **kwargs: Any) -> JSON:
+    def get_ledger_grant(self, ledger_id: str, ledger_grant_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
-        """Get credit grant.
+        """Get a single grant.
 
-        Get credit by key.
+        Gets the grant for a ledger by ID.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param credit_grant_id: A unique identifier for a credit grant. Required.
-        :type credit_grant_id: str
+        :param ledger_grant_id: A unique identifier for a ledger grant. Required.
+        :type ledger_grant_id: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -4072,16 +4071,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -4098,17 +4097,17 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_grant_request(
+        _request = build_get_ledger_grant_request(
             ledger_id=ledger_id,
-            credit_grant_id=credit_grant_id,
+            ledger_grant_id=ledger_grant_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
@@ -4130,25 +4129,25 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace
-    def void_credit_grant(  # pylint: disable=inconsistent-return-statements
-        self, credit_grant_id: str, ledger_id: str, **kwargs: Any
+    def void_ledger_grant(  # pylint: disable=inconsistent-return-statements
+        self, ledger_grant_id: str, ledger_id: str, **kwargs: Any
     ) -> None:
-        """Void credit grant.
+        """Void ledger grant.
 
-        Void a credit grant by ID. Partially or fully used credits cannot be voided.
-        Voided credits won't be applied to the subject's balance anymore.
+        Void a ledger grant by ID. Partially or fully used grants cannot be voided.
+        Voided grant won't be applied to the subject's balance anymore.
 
-        :param credit_grant_id: A unique identifier for a credit grant. Required.
-        :type credit_grant_id: str
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_grant_id: A unique identifier for a ledger grant. Required.
+        :type ledger_grant_id: str
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             409: ResourceExistsError,
@@ -4159,16 +4158,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        _request = build_void_credit_grant_request(
-            credit_grant_id=credit_grant_id,
+        _request = build_void_ledger_grant_request(
+            ledger_grant_id=ledger_grant_id,
             ledger_id=ledger_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
```

### Comparing `openmeter-1.0.0b72/src/openmeter/_operations/_patch.py` & `openmeter-1.0.0b73/src/openmeter/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_patch.py` & `openmeter-1.0.0b73/src/openmeter/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_serialization.py` & `openmeter-1.0.0b73/src/openmeter/_serialization.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/_vendor.py` & `openmeter-1.0.0b73/src/openmeter/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/__init__.py` & `openmeter-1.0.0b73/src/openmeter/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_client.py` & `openmeter-1.0.0b73/src/openmeter/aio/_client.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_configuration.py` & `openmeter-1.0.0b73/src/openmeter/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_operations/__init__.py` & `openmeter-1.0.0b73/src/openmeter/aio/_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_operations/_operations.py` & `openmeter-1.0.0b73/src/openmeter/aio/_operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,44 +19,44 @@
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
 from ..._operations._operations import (
-    build_create_credit_grant_request,
     build_create_feature_request,
+    build_create_ledger_grant_request,
     build_create_ledger_request,
     build_create_meter_request,
     build_create_portal_token_request,
     build_delete_feature_request,
     build_delete_meter_request,
     build_delete_subject_request,
-    build_get_credit_balance_request,
-    build_get_credit_grant_request,
-    build_get_credit_history_request,
     build_get_feature_request,
+    build_get_ledger_balance_request,
+    build_get_ledger_grant_request,
+    build_get_ledger_history_request,
     build_get_meter_request,
     build_get_subject_request,
     build_ingest_events_request,
     build_invalidate_portal_tokens_request,
-    build_list_credit_grants_by_ledger_request,
-    build_list_credit_grants_request,
     build_list_events_request,
     build_list_features_request,
+    build_list_ledger_grants_by_ledger_request,
+    build_list_ledger_grants_request,
     build_list_ledgers_request,
     build_list_meter_subjects_request,
     build_list_meters_request,
     build_list_portal_tokens_request,
     build_list_subjects_request,
     build_query_meter_request,
     build_query_portal_meter_request,
-    build_reset_credit_request,
+    build_reset_ledger_request,
     build_upsert_subject_request,
-    build_void_credit_grant_request,
+    build_void_ledger_grant_request,
 )
 from .._vendor import ClientMixinABC
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import MutableMapping  # type: ignore  # pylint: disable=ungrouped-imports
@@ -2288,15 +2288,15 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "id": "str",  # Readonly unique ULID identifier of the ledger.
                           Required.
                         "subject": "str",  # The metering subject this ledger used to track
-                          credits for. Required.
+                          grants for. Required.
                         "metadata": {
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         }
                     }
                 ]
         """
         error_map = {
@@ -2361,25 +2361,25 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
 
@@ -2400,15 +2400,15 @@
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
 
@@ -2425,25 +2425,25 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
 
                 # response body for status code(s): 201
                 response == {
                     "id": "str",  # Readonly unique ULID identifier of the ledger. Required.
-                    "subject": "str",  # The metering subject this ledger used to track credits
+                    "subject": "str",  # The metering subject this ledger used to track grants
                       for. Required.
                     "metadata": {
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     }
                 }
         """
         error_map = {
@@ -2498,23 +2498,23 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def get_credit_balance(
+    async def get_ledger_balance(
         self, ledger_id: str, *, time: Optional[datetime.datetime] = None, **kwargs: Any
     ) -> JSON:
         # pylint: disable=line-too-long
         """Get the balance of a specific subject.
 
         Get the balance of a specific subject.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword time: Point of time to query balances: date-time in RFC 3339 format. Defaults to now.
          Default value is None.
         :paramtype time: ~datetime.datetime
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -2554,19 +2554,18 @@
                                   :code:`<string>`.
                             },
                             "priority": 1,  # Optional. Default value is 1. The priority
                               of the grant. Grants with higher priority are applied first. Priority is
                               a positive decimal numbers. With lower numbers indicating higher
                               importance. For example, a priority of 1 is more urgent than a priority
                               of 2. When there are several grants available for the same subject, the
-                              system selects the grant with the highest priority. In cases where credit
-                              grants share the same priority level, the grant closest to its expiration
-                              will be used first. In the case of two credits have identical priorities
-                              and expiration dates, the system will use the grant that was created
-                              first.
+                              system selects the grant with the highest priority. In cases where grants
+                              share the same priority level, the grant closest to its expiration will
+                              be used first. In the case of two grants have identical priorities and
+                              expiration dates, the system will use the grant that was created first.
                             "rollover": {
                                 "type": "str",  # The rollover type to use:   *
                                   ``REMAINING_AMOUNT`` - Rollover remaining amount. *
                                   ``ORIGINAL_AMOUNT`` - Rollover re-applies the full grant amount.
                                   Required. Known values are: "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                                 "maxAmount": 0.0  # Optional. Maximum amount to
                                   rollover.
@@ -2601,15 +2600,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_balance_request(
+        _request = build_get_ledger_balance_request(
             ledger_id=ledger_id,
             time=time,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -2633,28 +2632,28 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def get_credit_history(
+    async def get_ledger_history(
         self,
         ledger_id: str,
         *,
         from_parameter: datetime.datetime,
         limit: int = 1000,
         to: Optional[datetime.datetime] = None,
         **kwargs: Any
     ) -> List[JSON]:
-        """Get credit ledger.
+        """Get the history of a ledger.
 
-        Get credit ledger for a specific subject.
+        Get the history of a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword from_parameter: Start of time range to query ledger: date-time in RFC 3339 format.
          Required.
         :paramtype from_parameter: ~datetime.datetime
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
         :keyword to: End of time range to query ledger: date-time in RFC 3339 format. Defaults to now.
@@ -2696,15 +2695,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_history_request(
+        _request = build_get_ledger_history_request(
             ledger_id=ledger_id,
             from_parameter=from_parameter,
             limit=limit,
             to=to,
             headers=_headers,
             params=_params,
         )
@@ -2730,23 +2729,23 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    async def reset_credit(
+    async def reset_ledger(
         self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
-        """Reset credit balance.
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Required.
         :type body: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
@@ -2754,37 +2753,37 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
 
     @overload
-    async def reset_credit(
+    async def reset_ledger(
         self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
-        """Reset credit balance.
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Required.
         :type body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
@@ -2792,48 +2791,48 @@
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
 
     @distributed_trace_async
-    async def reset_credit(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
-        """Reset credit balance.
+    async def reset_ledger(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+        """Reset the ledger's balance.
 
-        Resets the credit balances to zero for a specific subject and re-apply active grants with
+        Resets the ledger's balances to zero for a specific subject and re-apply active grants with
         rollover configuration.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :param body: Details for the reset. Is either a JSON type or a IO[bytes] type. Required.
         :type body: JSON or IO[bytes]
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
 
                 # response body for status code(s): 201
                 response == {
-                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the credit. It
+                    "effectiveAt": "2020-02-20 00:00:00",  # The time to reset the ledger. It
                       cannot be in the future. Required.
                     "id": "str"  # Readonly unique ULID identifier of the reset. Required.
                 }
         """
         error_map = {
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
@@ -2853,15 +2852,15 @@
         _json = None
         _content = None
         if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
-        _request = build_reset_credit_request(
+        _request = build_reset_ledger_request(
             ledger_id=ledger_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -2887,21 +2886,21 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def list_credit_grants(
+    async def list_ledger_grants(
         self, *, ledger_id: Optional[str] = None, limit: int = 1000, **kwargs: Any
     ) -> List[JSON]:
         # pylint: disable=line-too-long
-        """List credit grants for multiple ledgers.
+        """List grants for multiple ledgers.
 
-        List credit grants for multiple ledgers.
+        List grants for multiple ledgers.
 
         :keyword ledger_id: Filtering and group by multiple subjects.
 
          Usage: ``?ledgerID=01HX6VK5C498B3ABY9PR1069PP``. Default value is None.
         :paramtype ledger_id: str
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
@@ -2939,18 +2938,18 @@
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         },
                         "priority": 1,  # Optional. Default value is 1. The priority of the
                           grant. Grants with higher priority are applied first. Priority is a positive
                           decimal numbers. With lower numbers indicating higher importance. For
                           example, a priority of 1 is more urgent than a priority of 2. When there are
                           several grants available for the same subject, the system selects the grant
-                          with the highest priority. In cases where credit grants share the same
-                          priority level, the grant closest to its expiration will be used first. In
-                          the case of two credits have identical priorities and expiration dates, the
-                          system will use the grant that was created first.
+                          with the highest priority. In cases where grants share the same priority
+                          level, the grant closest to its expiration will be used first. In the case of
+                          two grants have identical priorities and expiration dates, the system will
+                          use the grant that was created first.
                         "rollover": {
                             "type": "str",  # The rollover type to use:   *
                               ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
                               Rollover re-applies the full grant amount. Required. Known values are:
                               "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                             "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                         }
@@ -2967,15 +2966,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_list_credit_grants_request(
+        _request = build_list_ledger_grants_request(
             ledger_id=ledger_id,
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -2999,21 +2998,21 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def list_credit_grants_by_ledger(self, ledger_id: str, *, limit: int = 1000, **kwargs: Any) -> List[JSON]:
+    async def list_ledger_grants_by_ledger(self, ledger_id: str, *, limit: int = 1000, **kwargs: Any) -> List[JSON]:
         # pylint: disable=line-too-long
-        """List credit grants.
+        """List ledger grants.
 
-        List credit grants for a specific ledger.
+        List ledger grants for a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :keyword limit: Number of entries to return. Default value is 1000.
         :paramtype limit: int
         :return: list of JSON object
         :rtype: list[JSON]
         :raises ~azure.core.exceptions.HttpResponseError:
 
@@ -3047,18 +3046,18 @@
                             "str": "str"  # Optional. Dictionary of :code:`<string>`.
                         },
                         "priority": 1,  # Optional. Default value is 1. The priority of the
                           grant. Grants with higher priority are applied first. Priority is a positive
                           decimal numbers. With lower numbers indicating higher importance. For
                           example, a priority of 1 is more urgent than a priority of 2. When there are
                           several grants available for the same subject, the system selects the grant
-                          with the highest priority. In cases where credit grants share the same
-                          priority level, the grant closest to its expiration will be used first. In
-                          the case of two credits have identical priorities and expiration dates, the
-                          system will use the grant that was created first.
+                          with the highest priority. In cases where grants share the same priority
+                          level, the grant closest to its expiration will be used first. In the case of
+                          two grants have identical priorities and expiration dates, the system will
+                          use the grant that was created first.
                         "rollover": {
                             "type": "str",  # The rollover type to use:   *
                               ``REMAINING_AMOUNT`` - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` -
                               Rollover re-applies the full grant amount. Required. Known values are:
                               "REMAINING_AMOUNT" and "ORIGINAL_AMOUNT".
                             "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                         }
@@ -3075,15 +3074,15 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[List[JSON]] = kwargs.pop("cls", None)
 
-        _request = build_list_credit_grants_by_ledger_request(
+        _request = build_list_ledger_grants_by_ledger_request(
             ledger_id=ledger_id,
             limit=limit,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
@@ -3107,25 +3106,25 @@
 
         if cls:
             return cls(pipeline_response, cast(List[JSON], deserialized), {})  # type: ignore
 
         return cast(List[JSON], deserialized)  # type: ignore
 
     @overload
-    async def create_credit_grant(
+    async def create_ledger_grant(
         self, ledger_id: str, body: JSON, *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Required.
+        :param body: The grant to create. Required.
         :type body: JSON
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -3152,16 +3151,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3191,40 +3190,40 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
                         "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                     }
                 }
         """
 
     @overload
-    async def create_credit_grant(
+    async def create_ledger_grant(
         self, ledger_id: str, body: IO[bytes], *, content_type: str = "application/json", **kwargs: Any
     ) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Required.
+        :param body: The grant to create. Required.
         :type body: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
@@ -3254,38 +3253,38 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
                         "maxAmount": 0.0  # Optional. Maximum amount to rollover.
                     }
                 }
         """
 
     @distributed_trace_async
-    async def create_credit_grant(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
+    async def create_ledger_grant(self, ledger_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
-        """Create credit grant.
+        """Create a grant on a specific ledger.
 
-        Creates a credit grant.
+        Create a grant on a specific ledger.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param body: The credit grant to create. Is either a JSON type or a IO[bytes] type. Required.
+        :param body: The grant to create. Is either a JSON type or a IO[bytes] type. Required.
         :type body: JSON or IO[bytes]
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
@@ -3309,16 +3308,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3348,16 +3347,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3384,15 +3383,15 @@
         _json = None
         _content = None
         if isinstance(body, (IOBase, bytes)):
             _content = body
         else:
             _json = body
 
-        _request = build_create_credit_grant_request(
+        _request = build_create_ledger_grant_request(
             ledger_id=ledger_id,
             content_type=content_type,
             json=_json,
             content=_content,
             headers=_headers,
             params=_params,
         )
@@ -3418,24 +3417,24 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def get_credit_grant(self, ledger_id: str, credit_grant_id: str, **kwargs: Any) -> JSON:
+    async def get_ledger_grant(self, ledger_id: str, ledger_grant_id: str, **kwargs: Any) -> JSON:
         # pylint: disable=line-too-long
-        """Get credit grant.
+        """Get a single grant.
 
-        Get credit by key.
+        Gets the grant for a ledger by ID.
 
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
-        :param credit_grant_id: A unique identifier for a credit grant. Required.
-        :type credit_grant_id: str
+        :param ledger_grant_id: A unique identifier for a ledger grant. Required.
+        :type ledger_grant_id: str
         :return: JSON object
         :rtype: JSON
         :raises ~azure.core.exceptions.HttpResponseError:
 
         Example:
             .. code-block:: python
 
@@ -3461,16 +3460,16 @@
                         "str": "str"  # Optional. Dictionary of :code:`<string>`.
                     },
                     "priority": 1,  # Optional. Default value is 1. The priority of the grant.
                       Grants with higher priority are applied first. Priority is a positive decimal
                       numbers. With lower numbers indicating higher importance. For example, a priority
                       of 1 is more urgent than a priority of 2. When there are several grants available
                       for the same subject, the system selects the grant with the highest priority. In
-                      cases where credit grants share the same priority level, the grant closest to its
-                      expiration will be used first. In the case of two credits have identical
+                      cases where grants share the same priority level, the grant closest to its
+                      expiration will be used first. In the case of two grants have identical
                       priorities and expiration dates, the system will use the grant that was created
                       first.
                     "rollover": {
                         "type": "str",  # The rollover type to use:   * ``REMAINING_AMOUNT``
                           - Rollover remaining amount. * ``ORIGINAL_AMOUNT`` - Rollover re-applies the
                           full grant amount. Required. Known values are: "REMAINING_AMOUNT" and
                           "ORIGINAL_AMOUNT".
@@ -3487,17 +3486,17 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[JSON] = kwargs.pop("cls", None)
 
-        _request = build_get_credit_grant_request(
+        _request = build_get_ledger_grant_request(
             ledger_id=ledger_id,
-            credit_grant_id=credit_grant_id,
+            ledger_grant_id=ledger_grant_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # type: ignore # pylint: disable=protected-access
@@ -3519,25 +3518,25 @@
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
     @distributed_trace_async
-    async def void_credit_grant(  # pylint: disable=inconsistent-return-statements
-        self, credit_grant_id: str, ledger_id: str, **kwargs: Any
+    async def void_ledger_grant(  # pylint: disable=inconsistent-return-statements
+        self, ledger_grant_id: str, ledger_id: str, **kwargs: Any
     ) -> None:
-        """Void credit grant.
+        """Void ledger grant.
 
-        Void a credit grant by ID. Partially or fully used credits cannot be voided.
-        Voided credits won't be applied to the subject's balance anymore.
+        Void a ledger grant by ID. Partially or fully used grants cannot be voided.
+        Voided grant won't be applied to the subject's balance anymore.
 
-        :param credit_grant_id: A unique identifier for a credit grant. Required.
-        :type credit_grant_id: str
-        :param ledger_id: A unique identifier for a credit ledger's subject. Required.
+        :param ledger_grant_id: A unique identifier for a ledger grant. Required.
+        :type ledger_grant_id: str
+        :param ledger_id: A unique identifier for a ledger. Required.
         :type ledger_id: str
         :return: None
         :rtype: None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             409: ResourceExistsError,
@@ -3548,16 +3547,16 @@
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = kwargs.pop("params", {}) or {}
 
         cls: ClsType[None] = kwargs.pop("cls", None)
 
-        _request = build_void_credit_grant_request(
-            credit_grant_id=credit_grant_id,
+        _request = build_void_ledger_grant_request(
+            ledger_grant_id=ledger_grant_id,
             ledger_id=ledger_id,
             headers=_headers,
             params=_params,
         )
         _request.url = self._client.format_url(_request.url)
 
         _stream = False
```

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_operations/_patch.py` & `openmeter-1.0.0b73/src/openmeter/aio/_operations/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_patch.py` & `openmeter-1.0.0b73/src/openmeter/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/src/openmeter/aio/_vendor.py` & `openmeter-1.0.0b73/src/openmeter/aio/_vendor.py`

 * *Files identical despite different names*

### Comparing `openmeter-1.0.0b72/PKG-INFO` & `openmeter-1.0.0b73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmeter
-Version: 1.0.0b72
+Version: 1.0.0b73
 Summary: Client for OpenMeter: Real-Time and Scalable Usage Metering
 Home-page: https://openmeter.io
 License: Apache-2.0
 Keywords: openmeter,api,client,usage,usage-based,metering,ai,aggregation,real-time,billing,cloud
 Author: Andras Toth
 Author-email: 4157749+tothandras@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

