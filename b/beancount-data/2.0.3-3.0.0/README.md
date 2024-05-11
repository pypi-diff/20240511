# Comparing `tmp/beancount_data-2.0.3.tar.gz` & `tmp/beancount_data-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_data-2.0.3.tar", max compression
+gzip compressed data, was "beancount_data-3.0.0.tar", max compression
```

## Comparing `beancount_data-2.0.3.tar` & `beancount_data-3.0.0.tar`

### file list

```diff
@@ -1,32 +1,5 @@
--rw-r--r--   0        0        0     1072 2024-01-04 04:14:37.542930 beancount_data-2.0.3/LICENSE
--rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/__init__.py
--rw-r--r--   0        0        0     3607 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/data_types.py
--rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/__init__.py
--rw-r--r--   0        0        0     1763 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Amount.py
--rw-r--r--   0        0        0     2990 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Balance.py
--rw-r--r--   0        0        0     2684 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Beancount.py
--rw-r--r--   0        0        0      188 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Booking.py
--rw-r--r--   0        0        0     1323 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Close.py
--rw-r--r--   0        0        0     1375 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Commodity.py
--rw-r--r--   0        0        0     2664 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Cost.py
--rw-r--r--   0        0        0     3636 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CostSpec.py
--rw-r--r--   0        0        0      163 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CostTypes.py
--rw-r--r--   0        0        0     2547 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Custom.py
--rw-r--r--   0        0        0     3347 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CustomValue.py
--rw-r--r--   0        0        0      182 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/CustomValueType.py
--rw-r--r--   0        0        0     1035 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Date.py
--rw-r--r--   0        0        0     3885 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Document.py
--rw-r--r--   0        0        0     3440 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Entry.py
--rw-r--r--   0        0        0      289 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/EntryPayload.py
--rw-r--r--   0        0        0     1757 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Event.py
--rw-r--r--   0        0        0     4825 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/MapItem.py
--rw-r--r--   0        0        0      189 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/MapValueType.py
--rw-r--r--   0        0        0     3765 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Note.py
--rw-r--r--   0        0        0     2790 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Open.py
--rw-r--r--   0        0        0     1769 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Pad.py
--rw-r--r--   0        0        0     5025 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Posting.py
--rw-r--r--   0        0        0     1749 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Price.py
--rw-r--r--   0        0        0     5673 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/Transaction.py
--rw-r--r--   0        0        0        0 2024-01-04 04:14:37.542930 beancount_data-2.0.3/beancount_data/fbs/data_types/__init__.py
--rw-r--r--   0        0        0      487 2024-01-04 04:14:37.542930 beancount_data-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 beancount_data-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-11 02:58:48.813445 beancount_data-3.0.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-11 02:58:48.813445 beancount_data-3.0.0/beancount_data/__init__.py
+-rw-r--r--   0        0        0     3736 2024-05-11 02:58:48.813445 beancount_data-3.0.0/beancount_data/data_types.py
+-rw-r--r--   0        0        0      444 2024-05-11 02:58:48.817445 beancount_data-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 beancount_data-3.0.0/PKG-INFO
```

### Comparing `beancount_data-2.0.3/LICENSE` & `beancount_data-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_data-2.0.3/beancount_data/data_types.py` & `beancount_data-3.0.0/beancount_data/data_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import decimal
 import enum
 import typing
 
 import pydantic
-from pydantic import Field
+from pydantic import ConfigDict
+from typing import Literal
 
 
 Account = str
 Flag = str
 Meta = typing.Dict[str, typing.Any]
 
 
@@ -33,124 +34,123 @@
     EVENT = "event"
     PRICE = "price"
     DOCUMENT = "document"
     CUSTOM = "custom"
 
 
 class BaseModel(pydantic.BaseModel):
-    class Config:
-        orm_mode = True
+    model_config = ConfigDict(from_attributes=True)
 
 
 class Amount(BaseModel):
-    number: typing.Optional[decimal.Decimal]
+    number: typing.Optional[decimal.Decimal] = None
     currency: str
 
 
 class EntryBase(BaseModel):
     meta: Meta
     date: datetime.date
 
 
 class Cost(BaseModel):
     number: decimal.Decimal
     currency: str
     date: datetime.date
-    label: typing.Optional[str]
+    label: typing.Optional[str] = None
 
 
 class CostSpec(BaseModel):
-    number_per: typing.Optional[decimal.Decimal]
-    number_total: typing.Optional[decimal.Decimal]
-    currency: typing.Optional[str]
+    number_per: typing.Optional[decimal.Decimal] = None
+    number_total: typing.Optional[decimal.Decimal] = None
+    currency: typing.Optional[str] = None
     date: datetime.date
-    label: typing.Optional[str]
-    merge: typing.Optional[bool]
+    label: typing.Optional[str] = None
+    merge: typing.Optional[bool] = None
 
 
 class Open(EntryBase):
-    entry_type: EntryType = Field(EntryType.OPEN, const=True)
+    entry_type: Literal[EntryType.OPEN] = EntryType.OPEN
     account: Account
-    currencies: typing.Optional[typing.List[str]]
-    booking: typing.Optional[Booking]
+    currencies: typing.Optional[typing.List[str]] = None
+    booking: typing.Optional[Booking] = None
 
 
 class Close(EntryBase):
-    entry_type: EntryType = Field(EntryType.CLOSE, const=True)
+    entry_type: Literal[EntryType.CLOSE] = EntryType.CLOSE
     account: Account
 
 
 class Commodity(EntryBase):
-    entry_type: EntryType = Field(EntryType.COMMODITY, const=True)
+    entry_type: Literal[EntryType.COMMODITY] = EntryType.COMMODITY
     currency: str
 
 
 class Pad(EntryBase):
-    entry_type: EntryType = Field(EntryType.PAD, const=True)
+    entry_type: Literal[EntryType.PAD] = EntryType.PAD
     account: Account
     source_account: str
 
 
 class Balance(EntryBase):
-    entry_type: EntryType = Field(EntryType.BALANCE, const=True)
+    entry_type: Literal[EntryType.BALANCE] = EntryType.BALANCE
     account: Account
     amount: Amount
-    tolerance: typing.Optional[decimal.Decimal]
-    diff_amount: typing.Optional[Amount]
+    tolerance: typing.Optional[decimal.Decimal] = None
+    diff_amount: typing.Optional[Amount] = None
 
 
 class Posting(BaseModel):
     account: Account
     units: Amount
-    cost: typing.Optional[typing.Union[Cost, CostSpec]]
-    price: typing.Optional[Amount]
-    flag: typing.Optional[Flag]
-    meta: typing.Optional[Meta]
+    cost: typing.Optional[typing.Union[Cost, CostSpec]] = None
+    price: typing.Optional[Amount] = None
+    flag: typing.Optional[Flag] = None
+    meta: typing.Optional[Meta] = None
 
 
 class Transaction(EntryBase):
-    entry_type: EntryType = Field(EntryType.TRANSACTION, const=True)
+    entry_type: Literal[EntryType.TRANSACTION] = EntryType.TRANSACTION
     flag: Flag
-    payee: typing.Optional[str]
+    payee: typing.Optional[str] = None
     narration: str
     tags: typing.Set[str]
     links: typing.Set[str]
     postings: typing.List[Posting]
 
 
 class Note(EntryBase):
-    entry_type: EntryType = Field(EntryType.NOTE, const=True)
+    entry_type: Literal[EntryType.NOTE] = EntryType.NOTE
     account: Account
     comment: str
     tags: typing.Set[str]
     links: typing.Set[str]
 
 
 class Event(EntryBase):
-    entry_type: EntryType = Field(EntryType.EVENT, const=True)
+    entry_type: Literal[EntryType.EVENT] = EntryType.EVENT
     type: str
     description: str
 
 
 class Price(EntryBase):
-    entry_type: EntryType = Field(EntryType.PRICE, const=True)
+    entry_type: Literal[EntryType.PRICE] = EntryType.PRICE
     currency: str
     amount: Amount
 
 
 class Document(EntryBase):
-    entry_type: EntryType = Field(EntryType.DOCUMENT, const=True)
+    entry_type: Literal[EntryType.DOCUMENT] = EntryType.DOCUMENT
     account: Account
     filename: str
     tags: typing.Set[str]
     links: typing.Set[str]
 
 
 class Custom(EntryBase):
-    entry_type: EntryType = Field(EntryType.CUSTOM, const=True)
+    entry_type: Literal[EntryType.CUSTOM] = EntryType.CUSTOM
     type: str
     values: typing.List[typing.Union[Amount, decimal.Decimal, str, bool]]
 
 
 EntryUnion = typing.Union[
     Open,
     Close,
@@ -165,12 +165,12 @@
     Custom,
 ]
 
 
 class ValidationError(BaseModel):
     source: Meta
     message: str
-    entry: typing.Optional[EntryUnion]
+    entry: typing.Optional[EntryUnion] = None
 
 
 class ValidationResult(BaseModel):
     errors: typing.List[ValidationError]
```

