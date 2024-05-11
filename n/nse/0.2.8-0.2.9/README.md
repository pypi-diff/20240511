# Comparing `tmp/nse-0.2.8.tar.gz` & `tmp/nse-0.2.9.tar.gz`

## Comparing `nse-0.2.8.tar` & `nse-0.2.9.tar`

### file list

```diff
@@ -1,42 +1,8 @@
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 nse-0.2.8/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nse-0.2.8/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 nse-0.2.8/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 nse-0.2.8/docs/make.bat
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 nse-0.2.8/docs/requirements.txt
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 nse-0.2.8/docs/source/conf.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 nse-0.2.8/docs/source/index.rst
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 nse-0.2.8/docs/source/usage.rst
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nse-0.2.8/src/__init__.py
--rw-r--r--   0        0        0    33706 2020-02-02 00:00:00.000000 nse-0.2.8/src/nse/NSE.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nse-0.2.8/src/nse/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/actions.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/advanceDecline.json
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/announcements.json
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/blockDeals.json
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/boardMeetings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/compileOptionChain.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/equityMetaInfo.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/equityQuote.json
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/fnoLots.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/gainers.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/holidays.json
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listCurrentIPO.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listEtf.json
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listFnoStocks.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listIndexStocks.json
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listIndices.json
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listPastIPO.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listSME.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listSgb.json
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/listUpcomingIPO.json
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/losers.json
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/optionChain.json
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/quote-trade_info.json
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/quote.json
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 nse-0.2.8/src/samples/status.json
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 nse-0.2.8/tests/Dockerfile
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 nse-0.2.8/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nse-0.2.8/LICENSE
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nse-0.2.8/README.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 nse-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 nse-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 nse-0.2.9/src/__init__.py
+-rw-r--r--   0        0        0    36081 2020-02-02 00:00:00.000000 nse-0.2.9/src/nse/NSE.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nse-0.2.9/src/nse/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 nse-0.2.9/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 nse-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 nse-0.2.9/README.md
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 nse-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 nse-0.2.9/PKG-INFO
```

### Comparing `nse-0.2.8/src/nse/NSE.py` & `nse-0.2.9/src/nse/NSE.py`

 * *Files 3% similar despite different names*

```diff
@@ -715,14 +715,84 @@
         )
 
         return self.__req(
             f"{self.base_url}/public-past-issues",
             params=params,
         ).json()
 
+    def circulars(
+        self,
+        dept_code: Optional[str] = None,
+        from_date: Optional[datetime] = None,
+        to_date: Optional[datetime] = None,
+    ) -> dict:
+        """
+        Return exchange circulars and communications by Department
+
+        `Sample response <https://github.com/BennyThadikaran/NseIndiaApi/blob/main/src/samples/circulars.json>`__
+
+        :param dept_code: Optional Department code. See table below for options
+        :param from_date: Optional defaults to 7 days from to_date
+        :type from_date: datetime.datetime
+        :param to_date: Optional defaults to current date
+        :type to_date: datetime.datetime
+        :raise ValueError: if `to_date` is less than `from_date`
+
+        Below is the list of `dept_code` values and their description
+
+        - CMTR - Capital Market (Equities) Trade
+        - COM - Commodity Derivatives
+        - CC - Corporate Communications
+        - CRM - CRM & Marketing
+        - CD - Currency Derivatives
+        - DS - Debt Segment
+        - SME - Emerge
+        - SMEITP - Emerge-ITP
+        - FAAC - Finance & Accounts
+        - FAO - Futures & Options
+        - INSP - Inspection & Compliance
+        - LEGL - Legal, ISC & Arbitration
+        - CMLS - Listing
+        - MA - Market Access
+        - MSD - Member Service Department
+        - MEMB - Membership
+        - MF - Mutual Fund
+        - NWPR - New Products
+        - NCFM - NSE Academy Limited
+        - CMPT - NSE Clearing - Capital Market
+        - IPO - Primary Market Segment
+        - RDM - Retail Debt Market
+        - SLBS - Securities Lending & Borrowing Scheme
+        - SURV - Surveillance & Investigation
+        - TEL - Systems & Telecom
+        - UCIBD - UCI Business Development
+        - WDTR - Wholesale Debt Market
+        """
+
+        if to_date is None:
+            to_date = datetime.now()
+
+        if from_date is None:
+            from_date = to_date - timedelta(7)
+
+        if to_date < from_date:
+            raise ValueError(
+                "Argument `to_date` cannot be less than `from_date`"
+            )
+
+        params = dict(
+            from_date=from_date.strftime("%d-%m-%Y"),
+            to_date=to_date.strftime("%d-%m-%Y"),
+        )
+
+        if dept_code:
+            params["dept"] = dept_code.upper()
+
+        return self.__req(f"{self.base_url}/circulars", params=params).json()
+
     def blockDeals(self) -> Dict:
         """Block deals
 
         `Sample response <https://github.com/BennyThadikaran/NseIndiaApi/blob/main/src/samples/blockDeals.json>`__
 
         :return: Block deals. ``data`` key is a list of all block deal (Empty list if no block deals).
         :rtype: dict"""
```

### Comparing `nse-0.2.8/.gitignore` & `nse-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nse-0.2.8/LICENSE` & `nse-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nse-0.2.8/README.md` & `nse-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nse-0.2.8/PKG-INFO` & `nse-0.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.3
 Name: nse
-Version: 0.2.8
+Version: 0.2.9
 Summary: Unofficial Python Api for NSE India stock exchange
 Project-URL: Homepage, https://github.com/BennyThadikaran/NseIndiaApi
 Project-URL: Bug Tracker, https://github.com/BennyThadikaran/NseIndiaApi/issues
 Author: Benny Thadikaran
 License-File: LICENSE
 Keywords: nse,nse-stock-data,stock-market-api,stock-news-api
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Office/Business :: Financial :: Investment
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Requires-Dist: mthrottle>=0.0.1
 Requires-Dist: requests>=2.31.0
 Description-Content-Type: text/markdown
 
 # 💰 NseIndiaApi
```

